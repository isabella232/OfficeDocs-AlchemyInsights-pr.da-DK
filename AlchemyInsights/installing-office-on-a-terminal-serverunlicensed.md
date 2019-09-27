---
title: Installation af Office på en Terminal Server-uden licens
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205403"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en Terminal Server

Til installation af Office 365 ProPlus på en Windows-Server ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:
  
- Du skal have en Office 365-plan, der omfatter Office 365 ProPlus, f. eks Office 365 Enterprise E3 eller Enterprise e5. Office 365 Business-og Office 365 Business Premium-planerne indeholder ikke Office 365 ProPlus.

- Du skal aktivere [delt computeraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Hvis du vil installere Office 365 ProPlus på RDS fra Microsoft 365 administration, ***som bruger standardindstillinger for installation***, skal du benytte følgende fremgangsmåde.

> [!TIP]
> Du kan også hente og køre [Microsofts support-og genoprettelsesassistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Office 365 ProPlus i den delte computer aktiveringstilstand.
  
1. Tjek, hvad Office 365 plan du har. [Lære](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Skift om nødvendigt til en anden Office 365-plan. [Lære](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Office 365-planer, skal du afinstallere det. For eksempel ved at gå til kontrol panel \> afinstallere et program. Afinstaller ved hjælp af [Microsofts support-og genoprettelsesassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du løber ind i problemer.

4. På RDS-serveren skal du logge på Microsoft 365 administration med din administratorkonto og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installeret, skal ***du ikke åbne eller logge*** på nogen Office-programmer.

6. Aktivér aktivering af delt computer på RDS-serveren ved at redigere registreringsdatabasen ved at følge disse trin:

1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg Kør. Skriv **regedit**i feltet Åbn, og vælg derefter OK.

2. Vælg Ja, når du bliver bedt om at tillade registrerings Editor at foretage ændringer på din enhed.

3. Tilføj en strengværdi af **Sharedcomputerlicensing** i registreringseditoren med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. ***Log på som en slutbruger*** på RDS-serveren, og [Bekræft, at aktivering af den delte computer er aktiveret for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Du kan finde flere oplysninger om forudsætninger, installationsvejledninger og vejledning om tilpassede installationer ved hjælp af Office-installationsværktøjet under [installere office 365 ProPlus ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Hvis du vil rette fejl i forbindelse med aktivering af delt computer, skal du se [fejlfinding af problemer med delt computeraktivering for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  