---
title: Installation af Microsoft 365 Apps for enterprise til delt brug på RDS, Terminal Server eller VDI
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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325597"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Installation af Microsoft 365 Apps for enterprise til delt brug på RDS, Terminal Server eller VDI

Sådan installeres Microsoft 365 Apps for enterprise fjernskrivebord-tjenester (RDS), tidligere kaldet Terminal Services:

- Du skal have en Microsoft 365 for Business-plan eller en Office 365 plan, der Microsoft 365 Apps for enterprise, f.eks. Office 365 Enterprise E3 eller Enterprise E5.
   **Bemærk!** Microsoft 365 Apps for business og Microsoft 365 Business Standard omfatter ikke Microsoft 365 Apps for enterprise.
- Du skal aktivere [aktivering af delt computer.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Bemærk!** Du kan også downloade og køre [Microsoft-programmet Support- og genoprettelsesassistent at](https://aka.ms/SaRA_OfficeSCA_M365Portal) installere Microsoft 365 Apps for enterprise i aktiveringstilstand for delt computer.

Du kan finde flere oplysninger om forudsætninger, konfigurationsinstruktioner og vejledning til tilpassede installationer ved hjælp af Office-udrulningsværktøjet i Installér Microsoft 365 Apps for enterprise ved hjælp af [Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Sådan retter du fejl i forbindelse med aktivering af delt computer:

- Se [Fejlfinding af problemer med aktivering af delt computer for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Se [Nulstil aktiveringstilstand for Microsoft 365-apps til store virksomheder](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere en Microsoft 365 Apps for enterprise på RDS fra den Microsoft 365 Administration, ***der*** bruger standardinstallationsindstillinger, skal du følge disse trin:

1. Kontrollér, hvilket abonnement du har. [Lær hvordan.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. Skift om nødvendigt til et andet abonnement. [Lær hvordan.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft-abonnementer, skal du fjerne den. Hvis du f.eks. går **til Kontrolpanel,**  >  **skal du fjerne et program.** Fjern ved [hjælp af Microsoft Support- og genoprettelsesassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du får problemer.
4. På RDS-serveren skal du logge på Microsoft 365 Administration med din administratorkonto og [installere Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. Når Office er installeret, ***skal du ikke åbne eller logge på*** nogen Office programmer.
6. På RDS-serveren skal du aktivere aktivering af delt computer ved at redigere registreringsdatabasen ved at følge disse trin:
   1. Højreklik på knappen Windows i nederste venstre hjørne af skærmen, og vælg **Kør.** I feltet Åbn skal du skrive **regedit** og derefter vælge **OK**.
   2. Vælg **Ja,** når du bliver bedt om at tillade registreringseditor at foretage ændringer på din enhed.
   3. I Registreringseditor skal du tilføje en strengværdi for **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. På RDS-serveren skal ***du logge på som slutbruger og*** bekræfte, at aktivering af delt computer er [aktiveret Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
