---
title: Installationen af office på en Terminal Server - uden licens
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498409"
---
# <a name="installing-office-on-a-terminal-server"></a>Installationen af Office på en Terminal Server

Til implementering af Office 365 ProPlus på en Windows-Server ved hjælp af Remote Desktop Services (RDS), tidligere kaldet Terminal Services:
  
- Du skal have en Office 365-plan, der indeholder Office 365 ProPlus, som Office 365 Enterprise E3 eller Enterprise E5. Business til Office 365 og Office 365 Business Premium planerne indeholder ikke Office 365 ProPlus.

- Du skal aktivere [delt computeraktivering](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Hvis du vil installere Office 365 ProPlus på RDS fra Office 365-portalen, ***som bruger standardindstillingerne for installation***, skal du følge disse trin:
  
1. Kontrollere, hvilke Office 365-plan, du har. [Lær, hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Hvis nødvendigt, Skift til en anden Office 365-planer. [Lær, hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Hvis Office er allerede installeret på RDS-serveren ved hjælp af andre Office 365-planer, kan du fjerne den. For eksempel ved at gå til Kontrolpanel \> afinstallerer et program. Fjern ved hjælp af [Microsoft Support og genoprettelse-assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) , hvis du kører i problemer.

4. Log på Office 365-portalen med administratorkonto og [installere Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)på RDS-serveren.

5. Når Office er installeret, ***ikke åbne eller logge på*** Office-programmer.

6. Aktiver delt computeraktivering på RDS-serveren, ved at redigere registreringsdatabasen ved at følge disse trin:

1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen og Vælg Kør. Skriv **regedit**i boksen Åbn, og klik derefter på OK.

2. Vælg Ja, når du bliver bedt om at tillade Registreringseditor til at foretage ændringer til din enhed.

3. I Registreringseditor, føje en strengværdi af **SharedComputerLicensing** med indstillingen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. På RDS-serveren, ***logge på som en slutbruger*** og [Kontroller, at delte computeraktivering er aktiveret for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Yderligere oplysninger om forudsætninger, installationsvejledning og vejledning om tilpassede installationer ved hjælp af værktøjet Office installation, finder du [Installere Office 365 ProPlus ved hjælp af Fjernskrivebord-tjenester](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
For at rette fejl, der er relateret til aktivering af delt computer, se [fejlfinding i forbindelse med problemer med aktivering af delt computer til Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  