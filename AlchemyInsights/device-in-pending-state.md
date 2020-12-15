---
title: Enhed i afventende tilstand
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677569"
---
# <a name="device-in-pending-state"></a>Enhed i afventende tilstand

**Forudsætninger**

1. Hvis du konfigurerer enheds registreringer for første gang, skal du sørge for, at du har gennemgået [Introduktion til Enhedsadministration i Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , der hjælper dig med at få enheder under kontrol af Azure ad.
2. Hvis du registrerer enheder i Azure AD direkte og tilmelder dem til Intune, skal du sikre dig, at du har [konfigureret Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) , og at [licensen](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) er placeret først.
3. Sørg for, at du har tilladelse til at udføre handlinger i Azure AD og i det lokale-annonce. Kun en global administrator i Azure AD kan administrere indstillinger for enheds registreringer. Hvis du er ved at konfigurere automatisk registrering i dit lokale Active Directory, skal du desuden være administrator af Active Directory og AD FS (hvis relevant).

Den hybride tilmelding til Azure AD join kræver, at der er enheder i virksomhedens netværk. Det fungerer også over VPN, men der er nogle uhensigtsmæssigheder til det. Vi har hørt, at kunder har brug for hjælp til fejlfinding i forbindelse med den hybride tilmelding til Azure AD join under fjernarbejde-omstændigheder.

**Skybaseret kryds godkendelses miljø (ved hjælp af Azure AD adgangskode-hash synkronisering eller pass-through-godkendelse)**

Dette registrerings forløb kaldes også "synkroniserings joinforbindelse".

Her er en oversigt over, hvad der sker under registreringsprocessen:

1. Windows 10 registrerer Service Connection Point-posten (SCP), når brugeren logger på enheden.

    1. Enheden forsøger først at hente lejer oplysninger fra klientside-SCP i registreringsdatabasen [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Du kan finde flere oplysninger i afsnittet [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Hvis den mislykkes, kommunikerer enheden med Active Directory lokalt for at få lejer oplysninger fra SCP. Hvis du vil bekræfte SCP, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Vi anbefaler, at du aktiverer SCP i Active Directory og kun bruger klient-SCP til indledende validering.

2. Windows 10 forsøger at kommunikere med Azure AD undersystem konteksten for at godkende sig selv over for Azure AD.

    Du kan kontrollere, om enheden kan få adgang til Microsoft-ressourcer undersystem kontoen ved hjælp af [scriptet til registrering af test af enhed](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genererer selvsigneret certifikat og gemmer det under computerobjektet i Active Directory lokalt. Dette forudsætter, at du har en oversigt over domænecontrolleren.

4. Enhedsobjekt, der har certifikatet, synkroniseret til Azure AD via Azure AD Connect. Synkroniseringscyklus er som standard hver 30 minut, men det afhænger af konfigurationen af Azure AD Connect. Hvis du vil have mere at vide, skal du se dette [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. På dette trin skal du kunne se emne enheden i tilstanden "**afventer**" under Device blade i Azure-portalen.

6. Næste gang du logger på Windows 10, bliver registreringen fuldført.

    > [!NOTE]
    > Hvis du er på VPN og logger af/logger på og afslutter domæne forbindelsen, kan du udløse registreringen manuelt. Sådan gør du:
    >
    > Udsted en `dsregcmd /join` lokal administrator prompt eller fjern via PsExec til din pc.
    >
    > F. eks.: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Du kan finde almindelige problemer med registrering af Azure Active Directory-enhed under [ofte stillede spørgsmål om enheder](https://docs.microsoft.com/azure/active-directory/devices/faq).
