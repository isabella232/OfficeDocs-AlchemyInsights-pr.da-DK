---
title: Installation Microsoft 365 Apps delt brug på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077244"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Installation Microsoft 365 Apps delt brug på RDS, Terminal Server eller VDI

For at Microsoft 365 Apps fjernskriveborde ved hjælp af RDS (Remote Desktop Services), tidligere Terminal Services, skal du:

- Brug den nemme løsning til at aktivere TLS 1.2 som standard, hvis du kører en ældre version af Windows (f.eks. Windows 7 SP1, Windows Server 2008 R2). For nem afhjælpning og flere oplysninger skal du se Opdater for at aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)som standard sikre protokoller i WinHTTP i Windows . 
- Have en plan, der Microsoft 365 Apps for enterprise (tidligere Office 365 Plus). For eksempel Office 365 E3 eller Microsoft 365 E5 eller en plan, der omfatter skrivebordsversionen af Project eller Visio, f.eks Project Plan 3 eller Visio Plan 2 eller Microsoft 365 Business Premium-planen, som også omfatter Microsoft 365 Apps for business.
- Aktivér aktivering af delt computer. Få mere at vide under [Oversigt over aktivering af delt computer for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Bemærk!** For at Microsoft 365 Apps i aktiveringstilstand for en delt computer skal du downloade og [køre Microsoft Support- og genoprettelsesassistent](https://aka.ms/SaRA_OfficeSCA_M365Portal). Hvis du vil have mere at vide om forudsætninger, konfigurationsinstruktioner og vejledning til at tilpasse installationer ved hjælp af Office-udrulningsværktøjet, skal du se Installér Microsoft 365 Apps ved hjælp af [Fjernskrivebord-tjenester](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

Hvis du vil rette fejl i forbindelse med aktivering af delt computer, skal du se:

- [Fejlfinding af problemer med aktivering af delt computer for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Nulstil Microsoft 365 Apps for enterprise aktiveringstilstand](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Hvis du vil installere en Microsoft 365 Apps på RDS fra den Microsoft 365 Administration, der bruger standardinstallationsindstillinger, skal du følge disse trin:

1. Kontrollér, Microsoft 365 plan du har. Du kan finde flere oplysninger [i Hvilket abonnement har jeg?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Skift om nødvendigt til en anden Microsoft 365 plan. Du kan få mere at vide [under Opgrader til en anden plan.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Hvis Microsoft 365 Apps allerede er installeret på RDS-serveren ved hjælp af andre inkompatible planer, skal du gå til Fjern  >  **et program i Kontrolpanel.** Hvis du løber ind i problemer, skal du fjerne ved [at downloade Microsoft Support- og genoprettelsesassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. På RDS-serveren skal du logge på Microsoft 365 Administration med din administratorkonto og [installere Office](https://portal.office.com/OLS/MySoftware.aspx).

   Når Office er installeret, skal du ikke åbne eller logge på nogen Office programmer.

1. På RDS-serveren skal du aktivere aktivering af delt computer ved at redigere registreringsdatabasen:

   1. Højreklik på Windows i nederste venstre hjørne af skærmen, og vælg **Kør.** I feltet Åbn skal du skrive **regedit** og derefter vælge **OK**.

   1. Når du bliver bedt om at tillade registreringseditor at foretage ændringer på din enhed, skal du **vælge Ja.**

   1. I Registreringseditor under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration skal du tilføje en strengværdi for **SharedComputerLicensing** med en indstilling på **1** .

1. På RDS-serveren skal du logge på som slutbruger og bekræfte, at aktivering af delt computer er aktiveret Microsoft 365 Apps. 

   Du kan få mere at vide [under Bekræft, at aktivering af delt computer er aktiveret Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).