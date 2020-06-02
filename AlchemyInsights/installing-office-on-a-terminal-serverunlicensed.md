---
title: Installation af kontor på en Terminal Server – Uden licens
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508622"
---
# <a name="installing-office-on-a-terminal-server"></a>Installere Office på en Terminal Server

Til installation af Microsoft 365 Apps til virksomheder på en Windows Server ved hjælp af RDS (Remote Desktop Services), tidligere kaldet Terminal Services:
  
- Du skal have et Microsoft 365-abonnement, der omfatter Microsoft 365 Apps til virksomheder, f.eks. Microsoft 365 Apps til virksomheder og Microsoft 365 Apps til virksomheder Premium-planer omfatter ikke Microsoft 365 Apps til virksomheder.

- Du skal aktivere aktivering af [delt computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Hvis du vil installere Microsoft 365 Apps til virksomheder på RDS fra Microsoft 365 Administration, ***som bruger standardinstallationsindstillinger***, skal du benytte følgende trin.

> [!TIP]
> Du kan også hente og køre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Microsoft 365 Apps til virksomheder i aktiveringstilstand for delte computere.
  
1. Se, hvilket Microsoft 365-abonnement du har. [Lære](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Skift om nødvendigt til et andet Microsoft 365-abonnement. [Lære](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft 365-abonnementer, skal du fjerne det. For eksempel ved at gå til Kontrolpanel \> Fjern et program. Fjern ved hjælp af [Microsoft Support and Recovery Assistant,](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du løber ind i problemer.

4. På RDS-serveren skal du logge på Microsoft 365 Administration med din administratorkonto og [installere Microsoft 365 Apps](https://portal.office.com/OLS/MySoftware.aspx)til virksomheder .

5. Når Office er installeret, ***må du ikke åbne eller logge på*** nogen Office-programmer.

6. Aktiver aktivering af delt computer på RDS-serveren ved at redigere registreringsdatabasen ved at fÃ ̧lge disse trin:

1. Højreklik på windows-knappen i nederste venstre hjørne af skærmen, og vælg Kør. Skriv **regedit**i feltet Åbn , og vælg derefter OK.

2. Vælg Ja, når du bliver bedt om at tillade, at Registreringseditor foretager ændringer på enheden.

3. Tilføj en strengværdi i **SharedComputerLicensing** i Registreringseditor med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. På RDS-serveren skal ***du logge på som slutbruger*** og kontrollere, at aktivering af delt computer er aktiveret for Microsoft [365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Du kan finde flere oplysninger om forudsætninger, konfigurationsinstruktioner og vejledning om tilpassede installationer ved hjælp af Office-installationsværktøjet under [Installere Microsoft 365 Apps til virksomheder ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Hvis du vil rette fejl i forbindelse med aktivering af delt computer, skal du se [Fejlfinding af problemer med aktivering af delte computere til Microsoft 365 Apps til virksomheder](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  