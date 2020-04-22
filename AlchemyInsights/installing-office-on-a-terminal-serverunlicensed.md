---
title: Installation af kontor på en Terminal Server - Uden licens
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763211"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en Terminal Server

Til installation af Microsoft 365 Apps til virksomheder på en Windows Server ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:
  
- Du skal have et Microsoft 365-abonnement, der omfatter Microsoft 365 Apps til virksomheder, f.eks. Microsoft 365 Apps til virksomheder og Microsoft 365 Apps til business Premium-planer omfatter ikke Microsoft 365 Apps til virksomheder.

- Du skal aktivere [aktivering af delt computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Hvis du vil installere Microsoft 365 Apps til virksomheder på RDS fra Microsoft 365 Administration, ***som bruger standardinstallationsindstillinger,*** skal du benytte følgende trin.

> [!TIP]
> Du kan også hente og køre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Microsoft 365 Apps til virksomheder i aktiveringstilstand for delt computer.
  
1. Se, hvilket Microsoft 365-abonnement du har. [Lære](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Skift om nødvendigt til et andet Microsoft 365-abonnement. [Lære](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft 365-abonnementer, skal du fjerne det. Ved at gå til \> Kontrolpanel Fjern et program. Fjern ved hjælp af [Microsoft Support and Recovery Assistant,](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du løber ind i problemer.

4. Log på Microsoft 365 Administration med din administratorkonto på RDS-serveren, og [installer Microsoft 365 Apps til virksomheder](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installeret, ***skal du ikke åbne eller logge på*** Office-programmer.

6. På RDS-serveren skal du aktivere delt computeraktivering ved at redigere registreringsdatabasen ved at følge disse trin:

1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg Kør. Skriv **regedit**i feltet Åbn , og vælg derefter OK.

2. Vælg Ja, når du bliver bedt om at tillade Registreringseditor at foretage ændringer på din enhed.

3. Tilføj en strengværdi af **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration i Registreringseditor.

7. Log på som ***slutbruger på*** RDS-serveren, og [kontroller, at aktivering af den delte computer er aktiveret for Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Yderligere oplysninger om forudsætninger, installationsvejledning og vejledning i tilpassede installationer ved hjælp af Office Deployment Tool finder du under [Installere Microsoft 365 Apps til virksomheder ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Hvis du vil rette fejl i forbindelse med aktivering af delte computere, skal du se [Fejlfinding af problemer med aktivering af delt computer for Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  