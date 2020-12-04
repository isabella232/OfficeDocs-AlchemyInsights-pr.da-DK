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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573381"
---
# <a name="troubleshoot-prt-issue"></a>Fejlfinding af PRT-problem

For at alle enheder kan fuldføres ved at blive ved med at blive fuldført, skal den være fuldt registeret og i god stand og kunne erhverve et primært PRT-token.

Hybrid registreringsprocessen for Azure AD join kræver, at enheder er på et virksomhedsnetværk. Det fungerer også over VPN, men der er nogle uhensigtsmæssigheder til det. Vi har hørt, at kunder har brug for hjælp til at foretage fejlfinding af hybrid Azure AD join-registreringsprocessen under fjernarbejde-omstændigheder. Her er en oversigt over, hvad der sker underliggende under processen.

**Skybaseret kryds godkendelses miljø (ved hjælp af Azure AD adgangskode-hash synkronisering eller pass-through-godkendelse)**

Dette registrerings forløb kaldes også "synkroniserings joinforbindelse".

1. Windows 10 registrerer en SCP-post, når brugeren logger på enheden.
    1. Enheden forsøger først at hente lejer oplysninger fra klientside-SCP i registreringsdatabasen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Hvis du vil have mere at vide, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Hvis den mislykkes, kommunikerer enheden med Active Directory lokalt (AD) for at få lejer oplysninger fra SCP (Service Connection Point). Hvis du vil bekræfte SCP, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Vi anbefaler, at du aktiverer SCP i ANNONCEn og kun bruger klient-SCP til indledende validering.

2. Windows 10 forsøger at kommunikere med Azure AD undersystem konteksten for at godkende sig selv over for Azure AD. Du kan kontrollere, om enheden kan få adgang til Microsoft-ressourcer undersystem kontoen ved hjælp af scriptet til registrering af test af enhed.

3. Windows 10 genererer et selvsigneret certifikat og gemmer det under computerobjektet i den lokale annonce. Dette forudsætter, at du har en oversigt over domænecontrolleren.

4. Et enhedsobjekt, der har et certifikat, bliver synkroniseret til Azure AD via Azure AD Connect. Synkroniseringscyklus er som standard hver 30 minut, men det afhænger af konfigurationen af Azure AD Connect. Hvis du vil have mere at vide, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. På dette trin skal du kunne se emne enheden i tilstanden "afventer" under Device blade i Azure-portalen.

6. Næste gang du logger på Windows 10, bliver registreringen fuldført. 

> [!NOTE]
> Hvis du bruger en VPN-forbindelse, og en logoff-logon-proces stopper domæne forbindelsen, kan du udløse registreringen manuelt:
 1. Udsted en dsregcmd/join lokalt på administrator prompt eller eksternt via PSExec til din PC. F. eks. PsExec-s \\ win10client01 cmd, dsregcmd/join

 2. Du kan finde flere oplysninger om problemer med hybrid deltagelse under [fejlfinding af problemer med enheder](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
