---
title: Installation af Microsoft 365-apps til virksomheder til delt brug på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200667"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Installation af Microsoft 365-apps til virksomheder til delt brug på RDS, Terminal Server eller VDI

Sådan installeres Microsoft 365-apps til virksomheder ved hjælp af Fjernskrivebord-tjenester (RDS), tidligere kaldet Terminal Services:

- Du skal have en Microsoft 365 til virksomheder-plan eller en Office 365-plan, der indeholder Microsoft 365-apps til virksomheder, f.eks. Office 365 Enterprise E3 eller Enterprise E5.
   > [!NOTE]
   > Microsoft 365-planer til virksomheder og Microsoft 365 Business Standard omfatter ikke Microsoft 365-apps til virksomheder.
- Du skal aktivere [aktivering af delt computer.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Du kan også downloade og køre [Microsoft Support-](https://aka.ms/SaRA_OfficeSCA_M365Portal) og genoprettelsesassistent for at installere Microsoft 365-apps til virksomheder i aktiveringstilstand for delt computer.

Du kan finde flere oplysninger om forudsætninger, konfigurationsvejledning og vejledning til tilpassede installationer ved hjælp af Office Udrulningsværktøj i Installér [Microsoft 365-apps](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)til virksomheder ved hjælp af Fjernskrivebord-tjenester.

Sådan retter du fejl i forbindelse med aktivering af delt computer:

- Se [Fejlfinding af problemer med aktivering af delt computer til Microsoft 365-apps til virksomheder.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Se [Nulstil aktiveringstilstand for Microsoft 365-apps til store virksomheder](https://go.microsoft.com/fwlink/?linkid=2109218).

Hvis du vil installere Microsoft 365 Apps til virksomheder på RDS fra Microsoft 365 ***Administration,*** der bruger standardinstallationsindstillinger, skal du følge disse trin:

1. Kontrollér, hvilket abonnement du har. [Se hvordan.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)
2. Skift til et andet abonnement, hvis det er nødvendigt. [Se hvordan.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)
3. Hvis Office allerede er installeret på RDS-serveren ved hjælp af andre Microsoft-abonnementer, skal du fjerne det. Ved f.eks. at **gå til Kontrolpanel skal du** fjerne et  >  **program.** Fjern ved [hjælp af Microsoft Support- og](https://aka.ms/SARA-OfficeUninstall-Alchemy) genoprettelsesassistent, hvis du får problemer.
4. På RDS-serveren skal du logge på Microsoft 365 Administration med din administratorkonto og installere [Microsoft 365-apps til virksomheder.](https://portal.office.com/OLS/MySoftware.aspx)
5. Når Office er installeret, ***skal du ikke åbne eller logge på nogen*** Office-programmer.
6. Aktivér aktivering af delt computer på RDS-serveren ved at redigere registreringsdatabasen ved at følge disse trin:
   1. Højreklik på Windows-knappen i nederste venstre hjørne af skærmen, og vælg **Kør.** Skriv **regedit** i feltet Åbn, og vælg derefter **OK.**
   2. Vælg **Ja,** når du bliver bedt om at tillade Registreringseditor at foretage ændringer på din enhed.
   3. I Registreringseditor skal du tilføje en strengværdi for **SharedComputerLicensing** med en indstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Log på som  slutbruger på RDS-serveren, og bekræft, at aktivering af delt computer er aktiveret [for Microsoft 365-apps til virksomheder.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
