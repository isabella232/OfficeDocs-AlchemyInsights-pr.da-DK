---
title: Enhed i ventende tilstand
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330366"
---
# <a name="device-in-pending-state"></a>Enhed i ventende tilstand

**Forudsætninger:**

1. Hvis du konfigurerer enhedsregistreringer for første gang, skal du kontrollere, at du har gennemgået Introduktion til enhedshåndtering i [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) der kan hjælpe dig med at få enheder under kontrol af Azure AD.
2. Hvis du registrerer enheder direkte i Azure AD og tilmelder dem i Intune, skal du sikre dig, at du har konfigureret [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og har licensen på plads først. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)
3. Sørg for, at du er godkendt til at udføre handlinger i Azure AD og i det lokale AD. Kun en global administrator i Azure AD kan administrere indstillingerne for enhedsregistreringer. Hvis du konfigurerer automatiske registreringer i dit lokale Active Directory, skal du desuden være administrator for Active Directory og AD FS (hvis det er relevant).

Registreringsprocessen for hybrid Azure AD-tilmelding kræver, at enheder er på virksomhedens netværk. Det fungerer også via VPN, men der er nogle problemer med det. Vi har hørt, at kunder har brug for hjælp til fejlfinding af registreringsprocessen for Azure AD-tilmeldinger i forbindelse med fjernarbejde.

**Skygodkendelsesmiljø (ved hjælp af Azure AD-synkronisering af adgangskodehash eller pass-through-godkendelse)**

Denne registreringsstrøm kaldes også "Synkroniser join".

Her er en oversigt over, hvad der sker under registreringsprocessen:

1. Windows 10 opdager Service Connection Point (SCP)-posten, når brugeren logger på enheden.

    1. Enheden forsøger først at hente lejeroplysninger fra klientsiden SCP i registreringsdatabasen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Du kan finde flere oplysninger i [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Hvis det ikke lykkes, kommunikerer enheden med det lokale Active Directory for at få lejeroplysninger fra SCP. Se dette dokument for [](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)at bekræfte SCP.

    **Bemærk!** Vi anbefaler, at du aktiverer SCP i Active Directory og kun bruger SCP på klientsiden til indledende validering.

2. Windows 10 forsøger at kommunikere med Azure AD i systemkonteksten for at godkende sig selv i forhold til Azure AD.

    Du kan kontrollere, om enheden kan få adgang til Microsoft-ressourcer under systemkontoen ved hjælp af [scriptet Test enhedsregistreringsforbindelse](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genererer et selv signeret certifikat og gemmer det under computerobjektet i det lokale Active Directory. Dette kræver, at du bruger domænecontroller.

4. Enhedsobjekt, der har certifikat, synkroniseres med Azure AD via Azure AD Forbind. Synkroniseringscyklussen er som standard hvert 30. minut, men det afhænger af konfigurationen af Azure AD Forbind. Du kan finde flere oplysninger i dette [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. På dette tidspunkt bør du kunne se emneenheden i tilstanden "**Afventer"** under Enheds bladet for Azure Portal.

6. Ved næste brugerlogon på Windows 10, fuldføres registreringen.

    **Bemærk!** Hvis du bruger VPN, og logoff/logon afslutter domæneforbindelsen, kan du udløse registrering manuelt. Sådan gør du:
    
    Problem med `dsregcmd /join` en lokal administratorprompt eller eksternt via PSExec til din pc.\
    For eksempel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Se Ofte stillede spørgsmål om Azure Active Directory enheder for almindelige problemer [med registrering af enheder.](https://docs.microsoft.com/azure/active-directory/devices/faq)
