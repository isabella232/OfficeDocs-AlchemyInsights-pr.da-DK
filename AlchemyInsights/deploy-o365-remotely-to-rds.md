---
title: Installation af Microsoft 365-apps til virksomheder til delt brug på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786271"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Installation af Microsoft 365-apps til virksomheder til delt brug på RDS, Terminal Server eller VDI

Sådan installerer du Microsoft 365-apps til virksomheder ved hjælp af Fjernskrivebord-tjenester (RDS), tidligere kaldet Terminal Services:
- Du skal have en Microsoft 365 til virksomheder-plan eller en Office 365-plan, der omfatter Microsoft 365-apps til Enterprise, f. eks Office 365 Enterprise E3 eller Enterprise e5.
   > [!NOTE] 
   > Microsoft 365-apps til virksomheder og standard planer for Microsoft 365 Business Premium omfatter ikke Microsoft 365-apps til Enterprise.
- Du skal aktivere [delt computeraktivering](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Du kan også downloade og køre [Microsoft support-og genoprettelses assistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Microsoft 365-apps til virksomheder i aktiveringstilstand for delt computer.

Du kan finde flere oplysninger om forudsætninger, konfigurations instruktioner og vejledning til brugerdefinerede installationer ved hjælp af Office-udrulnings værktøjet under [installere Microsoft 365-apps til Enterprise ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Sådan løser du fejl, der er relateret til aktivering af delt computer:
- Se [fejlfinding af problemer med delt computeraktivering for Microsoft 365-apps til Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Se [Nulstil aktiveringstilstand for Microsoft 365-apps til store virksomheder](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365-apps til Enterprise på RDS fra Microsoft 365 administration, ***som bruger standard installationsindstillinger***, skal du følge disse trin:

1.    Kontrollér, hvilket abonnement du har. [Lær hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Hvis det er nødvendigt, kan du skifte til et andet abonnement. [Lær hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft-abonnementer, skal du fjerne det. For eksempel ved at gå til **kontrolpanelet**  >  **Fjern et program**. Fjern med [Microsoft support-og genoprettelses assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du kører i problemer.
4.    På RDS-serveren skal du logge på Microsoft 365 administration med din administratorkonto og [installere Microsoft 365-apps til Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Når Office er installeret, skal du ***ikke åbne eller logge på*** nogen Office-programmer.
6.    På RDS-serveren skal du aktivere delt computeraktivering ved at redigere registreringsdatabasen ved at følge disse trin:
   1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg **Kør**. Skriv **regedit**i feltet Åbn, og vælg derefter **OK**.
   2. Vælg **Ja** , når du bliver bedt om at tillade, at registrerings Editor foretager ændringer på din enhed.
   3. I registrerings Editor skal du tilføje en strengværdi for **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. På RDS-serveren skal du ***logge på som en slutbruger*** og [bekræfte, at aktivering af delt computer er aktiveret for Microsoft 365-apps til Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

