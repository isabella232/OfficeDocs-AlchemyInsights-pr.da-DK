---
title: Installation af Microsoft 365-apps til virksomheder til delt brug på RDS, Terminal Server eller VDI
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507580"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Installation af Microsoft 365-apps til virksomheder til delt brug på RDS, Terminal Server eller VDI

Sådan installeres Microsoft 365 Apps til virksomheder ved hjælp af RDS (Remote Desktop Services), der tidligere hed Terminal Services:
- Du skal have en Microsoft 365 For Business-plan eller en Office 365-plan, der omfatter Microsoft 365 Apps til virksomheder, f.eks.
   > [!NOTE] 
   > Microsoft 365 Apps til virksomheder og Microsoft 365 Business Premium Standard-planer omfatter ikke Microsoft 365 Apps til virksomheder.
- Du skal aktivere [aktivering af delt computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Du kan også hente og køre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Microsoft 365 Apps til virksomheder i aktiveringstilstand for delte computere.

Du kan finde flere oplysninger om forudsætninger, konfigurationsinstruktioner og vejledning om tilpassede installationer ved hjælp af Office Installationsværktøj i [Installere Microsoft 365 Apps til virksomheder ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Sådan rettes fejl i forbindelse med aktivering af delt computer:
- Se [Fejlfinding af problemer med aktivering af delte computere til Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Se [Nulstil aktiveringstilstand for Microsoft 365-apps til store virksomheder](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365 Apps til virksomheder på RDS fra Microsoft 365 Administration, ***som bruger standardinstallationsindstillinger***, skal du benytte følgende fremgangsmåde:

1.    Se, hvilket abonnement du har. [Få mere at vide om, hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Skift om nødvendigt til et andet abonnement. [Få mere at vide om, hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft-abonnementer, skal du fjerne det. Ved at gå til **Kontrolpanel**  >  **Fjern et program**. Fjern ved hjælp af [Microsoft Support and Recovery Assistant,](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du løber ind i problemer.
4.    På RDS-serveren skal du logge på Microsoft 365 Administration med din administratorkonto og [installere Microsoft 365 Apps](https://portal.office.com/OLS/MySoftware.aspx)til virksomheder .
5.    Når Office er installeret, ***må du ikke åbne eller logge på*** nogen Office-programmer.
6.    Aktiver aktivering af delt computer på RDS-serveren ved at redigere registreringsdatabasen ved at fÃ ̧lge disse trin:
   1. Højreklik på windows-knappen i nederste venstre hjørne af skærmen, og vælg **Kør**. Skriv **regedit**i feltet Åbn , og vælg derefter **OK**.
   2. Vælg **Ja,** når du bliver bedt om at tillade, at Registreringseditor foretager ændringer på enheden.
   3. Tilføj en strengværdi i **SharedComputerLicensing** i Registreringseditor med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. På RDS-serveren skal ***du logge på som slutbruger*** og kontrollere, at aktivering af delt computer er aktiveret for Microsoft [365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

