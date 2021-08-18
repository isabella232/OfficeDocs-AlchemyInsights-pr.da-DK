---
title: Installation af Office på en Terminal Server – uden licens
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321993"
---
# <a name="installing-office-on-a-terminal-server"></a>Installation af Office på en Terminal Server

Udrulning Microsoft 365 Apps for enterprise en Windows server ved hjælp af RDS (Remote Desktop Services), tidligere kaldet Terminal Services:
  
- Du skal have et Microsoft 365, der omfatter Microsoft 365 Apps for enterprise, f.eks. Office 365 Enterprise E3 eller Enterprise E5. De Microsoft 365 Apps for business og Microsoft 365 Apps for business Premium omfatter ikke Microsoft 365 Apps for enterprise.

- Du skal aktivere aktivering [af delt computer.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Hvis du vil installere en Microsoft 365 Apps for enterprise på RDS fra den Microsoft 365 Administration, der bruger ***standardinstallationsindstillinger***, skal du følge disse trin.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Kontrollér, Microsoft 365-abonnement du har. [Sådan gør du](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Skift om nødvendigt til et andet Microsoft 365 abonnement. [Sådan gør du](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft 365,skal du fjerne den. Hvis du f.eks. vil gå til Kontrolpanel, \> skal du fjerne et program. Fjern ved [hjælp af Microsoft Support- og genoprettelsesassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du får problemer.

4. På RDS-serveren skal du logge på Microsoft 365 Administration med din administratorkonto og [installere Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installeret, ***skal du ikke åbne eller logge på*** nogen Office programmer.

6. På RDS-serveren skal du aktivere aktivering af delt computer ved at redigere registreringsdatabasen ved at følge disse trin:

1. Højreklik på Windows i nederste venstre hjørne af skærmen, og vælg Kør. Skriv **regedit** i feltet Åbn, og vælg derefter OK.

2. Vælg Ja, når du bliver bedt om at tillade registreringseditor at foretage ændringer på din enhed.

3. I Registreringseditor skal du tilføje en strengværdi for **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. På RDS-serveren skal ***du logge på som slutbruger*** og bekræfte, at aktivering af delt computer er [aktiveret Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Hvis du vil have mere at vide om forudsætninger, konfigurationsinstruktioner og vejledning til tilpassede installationer ved hjælp af Office-udrulningsværktøjet, skal du se Installér Microsoft 365 Apps for enterprise ved hjælp af [Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Hvis du vil løse fejl i forbindelse med aktivering af delt computer, skal du se [Fejlfinding i forbindelse med problemer med aktivering af delt computer Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  