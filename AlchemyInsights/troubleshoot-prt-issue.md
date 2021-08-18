---
title: Fejlfinding af PRT-problem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330953"
---
# <a name="troubleshoot-prt-issue"></a>Fejlfinding af PRT-problem

Hvis en enhed skal være godkendt, skal den være fuldt registreret og i god stand og kunne få et primært opdateringstoken (PRT).

Registreringsprocessen for Azure AD-hybridtilmelding kræver, at enheder er på et virksomhedsnetværk. Det fungerer også via VPN, men der er nogle problemer med det. Vi har hørt, at kunder har brug for hjælp til fejlfinding i forbindelse med registreringsprocessen af hybride Azure AD-tilmeldinger under fjernarbejde. Her er en oversigt over, hvad der sker under registreringsprocessen.

**Skygodkendelsesmiljø (ved hjælp af Azure AD-synkronisering af adgangskodehash eller pass-through-godkendelse)**

Denne registreringsstrøm kaldes også "Synkroniser join".

1. Windows 10 opdager en SCP-post, når brugeren logger på enheden.
    1. Enheden forsøger først at hente lejeroplysninger fra klientsiden SCP i registreringsdatabasen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Du kan finde flere oplysninger i dette [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Hvis det ikke lykkes, kommunikerer enheden med Active Directory (AD) i det lokale miljø for at få lejeroplysninger fra Service Connection Point (SCP). Hvis du vil bekræfte SCP, skal du se dette [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Bemærk!** Vi anbefaler, at du aktiverer SCP i AD og kun bruger SCP på klientsiden til indledende validering.

2. Windows 10 forsøger at kommunikere med Azure AD i systemkonteksten for at godkende sig selv i forhold til Azure AD. Du kan kontrollere, om enheden kan få adgang til Microsoft-ressourcer under systemkontoen ved hjælp af scriptet Test enhedsregistreringsforbindelse.

3. Windows 10 genererer et selv signeret certifikat og gemmer det under computerobjektet i det lokale AD. Dette kræver, at du bruger domænecontroller.

4. Et enhedsobjekt, der har et certifikat, synkroniseres med Azure AD via Azure AD Forbind. Synkroniseringscyklussen er som standard hvert 30. minut, men det afhænger af konfigurationen af Azure AD Forbind. Du kan finde flere oplysninger i dette [dokument.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. På dette tidspunkt bør du kunne se emneenheden i "Afventende" tilstand under Enheds bladet for Azure Portal.

6. Ved næste brugerlogon på Windows 10, fuldføres registreringen. 

**Bemærk!** Hvis du bruger VPN, og en logoff-logonproces afslutter domæneforbindelsen, kan du udløse registrering manuelt:
 1. Udse en dsregcmd /join lokalt på administratorprompt eller eksternt via PSExec til din pc. For eksempel PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Du kan få mere at vide om hybridforbindelsesproblemer under [Fejlfinding af problemer med enheder.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
