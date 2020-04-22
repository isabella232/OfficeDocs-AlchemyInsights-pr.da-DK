---
title: Installation af Microsoft 365 Apps til virksomheder til delt brug på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704699"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Installation af Microsoft 365 Apps til virksomheder til delt brug på RDS, Terminal Server eller VDI

Sådan installeres Microsoft 365 Apps til virksomheder ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:
- Du skal have en Microsoft 365 Til Business-plan eller en Office 365-plan, der indeholder Microsoft 365 Apps til virksomheder, f.eks.
   > [!NOTE] 
   > Microsoft 365 Apps til virksomheder og Microsoft 365 Business Premium Standard-planerne omfatter ikke Microsoft 365 Apps til virksomheder.
- Du skal aktivere [aktivering af delt computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Du kan også hente og køre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Microsoft 365 Apps til virksomheder i aktiveringstilstand for delt computer.

Yderligere oplysninger om forudsætninger, installationsinstruktioner og vejledning i tilpassede installationer ved hjælp af Office Deployment Tool finder du [under Installere Microsoft 365 Apps til virksomheder ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Sådan rettes fejl i forbindelse med aktivering af delt computer:
- Se [Fejlfinding af problemer med aktivering af delt computer for Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Se [Nulstil aktiveringstilstand for Microsoft 365-apps til store virksomheder](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365 Apps til virksomheder på RDS fra Microsoft 365 Administration, ***som bruger standardinstallationsindstillinger,*** skal du benytte følgende fremgangsmåde:

1.    Se, hvilket abonnement du har. [Få mere at vide om, hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)du finder ud af
2.    Skift om nødvendigt til et andet abonnement. [Få mere at vide om, hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)du finder ud af
3.    Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft-abonnementer, skal du fjerne det. Ved at gå til **Kontrolpanel** > **Fjern et program**. Fjern ved hjælp af [Microsoft Support and Recovery Assistant,](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du løber ind i problemer.
4.    Log på Microsoft 365 Administration med din administratorkonto på RDS-serveren, og [installer Microsoft 365 Apps til virksomheder](https://portal.office.com/OLS/MySoftware.aspx).
5.    Når Office er installeret, ***skal du ikke åbne eller logge på*** Office-programmer.
6.    På RDS-serveren skal du aktivere delt computeraktivering ved at redigere registreringsdatabasen ved at følge disse trin:
   1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg **Kør**. Skriv **regedit**i feltet Åbn , og vælg derefter **OK**.
   2. Vælg **Ja,** når du bliver bedt om at tillade Registreringseditor at foretage ændringer på din enhed.
   3. Tilføj en strengværdi af **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration i Registreringseditor.
   4. Log på som ***slutbruger på*** RDS-serveren, og [kontroller, at aktivering af den delte computer er aktiveret for Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

