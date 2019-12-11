---
title: Implementering af Office 365 ProPlus til delt brug på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959454"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementering af Office 365 ProPlus til delt brug på RDS, Terminal Server eller VDI

Sådan implementeres Office 365 ProPlus ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:
- Du skal have en Microsoft 365 for business-plan eller en Office 365-plan, der omfatter Office 365 ProPlus, såsom Office 365 Enterprise E3 eller Enterprise e5.
   > [!NOTE] 
   > Office 365 Business-og Office 365 Business Premium-planerne indeholder ikke Office 365 ProPlus.
- Du skal aktivere [Aktivering af delt computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Du kan også hente og køre [Microsofts support-og genoprettelsesassistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Office 365 ProPlus i den delte computer aktiveringstilstand.

Du finder flere oplysninger om forudsætninger, installationsvejledninger og vejledning om tilpassede installationer ved hjælp af Office-installationsværktøjet under [implementere office 365 ProPlus ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Sådan rettes fejl i forbindelse med aktivering af delt computer:
- Se [fejlfinding af problemer med delt computeraktivering for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Se [Nulstil Office 365 ProPlus-aktiveringstilstand](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Office 365 ProPlus på RDS fra Microsoft 365 administration, ***som bruger standardindstillinger for installation***, skal du benytte følgende fremgangsmåde:

1.  Tjek, hvad Office 365 plan du har. [Lær hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Skift om nødvendigt til en anden Office 365-plan. [Lær hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Office 365-planer, skal du afinstallere det. For eksempel ved at gå til **kontrol panel** > **afinstallere et program**. Afinstaller ved hjælp af [Microsofts support-og genoprettelsesassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du løber ind i problemer.
4.  På RDS-serveren skal du logge på Microsoft 365 administration med din administratorkonto og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Når Office er installeret, skal ***du ikke åbne eller logge*** på nogen Office-programmer.
6.  Aktivér aktivering af delt computer på RDS-serveren ved at redigere registreringsdatabasen ved at følge disse trin:
   1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg **Kør**. Skriv **regedit**i feltet Åbn, og vælg derefter **OK**.
   2. Vælg **Ja** , når du bliver bedt om at tillade registrerings Editor at foretage ændringer på din enhed.
   3. Tilføj en strengværdi af **Sharedcomputerlicensing** i registreringseditoren med en indstilling på 1 under HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. ***Log på som en slutbruger*** på RDS-serveren, og [Bekræft, at aktivering af den delte computer er aktiveret for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

