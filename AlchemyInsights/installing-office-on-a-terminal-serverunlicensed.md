---
title: Installation af Office på en Terminal Server uden licens
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663111"
---
# <a name="installing-office-on-a-terminal-server"></a>Installation af Office på en Terminal Server

Til installation af Microsoft 365-apps til virksomheder på en Windows-Server, der bruger Fjernskrivebord-tjenester (RDS), tidligere kaldet Terminal Services:
  
- Du skal have et Microsoft 365-abonnement, der omfatter Microsoft 365-apps til Enterprise, f. eks Office 365 Enterprise E3 eller Enterprise e5. Microsoft 365-apps til virksomheder og Microsoft 365-apps til Business Premium-planer omfatter ikke Microsoft 365-apps til Enterprise.

- Du skal aktivere [Aktivering af delt computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Hvis du vil installere Microsoft 365-apps til Enterprise på RDS fra Microsoft 365 administration, ***som bruger standard installationsindstillinger***, skal du følge disse trin.

> [!TIP]
> Du kan også downloade og køre [Microsoft support-og genoprettelses assistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) for at installere Microsoft 365-apps til virksomheder i aktiveringstilstand for delt computer.
  
1. Kontrollér, hvilket Microsoft 365-abonnement du har. [Lær hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Hvis det er nødvendigt, kan du skifte til et andet Microsoft 365-abonnement. [Lær hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Hvis Office allerede er installeret på RDS-serveren med andre Microsoft 365-abonnementer, skal du fjerne det. For eksempel ved at gå til kontrolpanelet \> Fjern et program. Fjern med [Microsoft support-og genoprettelses assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du kører i problemer.

4. På RDS-serveren skal du logge på Microsoft 365 administration med din administratorkonto og [installere Microsoft 365-apps til Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Når Office er installeret, skal du ***ikke åbne eller logge på*** nogen Office-programmer.

6. På RDS-serveren skal du aktivere delt computeraktivering ved at redigere registreringsdatabasen ved at følge disse trin:

1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg Kør. Skriv **regedit**i feltet Åbn, og vælg derefter OK.

2. Vælg Ja, når du bliver bedt om at tillade, at registrerings Editor foretager ændringer på din enhed.

3. I registrerings Editor skal du tilføje en strengværdi for **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. På RDS-serveren skal du ***logge på som en slutbruger*** og [bekræfte, at aktivering af delt computer er aktiveret for Microsoft 365-apps til Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Hvis du vil have mere at vide om forudsætninger, konfigurationsvejledning og vejledning til brugerdefinerede installationer ved hjælp af Office-udrulnings værktøjet, skal du se [installere Microsoft 365-apps til Enterprise ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Hvis du vil rette fejl, der er relateret til aktivering af delt computer, skal du se [fejlfinding af problemer med aktivering af delt computer for Microsoft 365-apps til Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  