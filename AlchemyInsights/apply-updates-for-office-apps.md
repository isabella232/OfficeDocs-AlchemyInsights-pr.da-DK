---
title: Anvend opdateringer til Office apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: 418c1166560b33c445d7ec452caadaa2295b87cc4766e7d36b7d711abb81a48e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969379"
---
# <a name="apply-updates-for-office-apps"></a>Anvend opdateringer til Office apps

Opdateringer til apps Office som standard gratis, downloades automatisk og anvendes i baggrunden uden brugerens indlæg. Hvis du vil køre opdateringer manuelt, hvis du får problemer med at anvende opdateringer, skal [du se Office opdateringer.](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5) Du kan få mere at vide [under Fejlfinding i forbindelse med installation Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).

Hvis du vil Office opdateringer til dine brugere, skal du overveje disse muligheder:

- Vælg den rette Office for din organisation baseret på den ønskede hyppighed af opdateringer. Hvis du vil se hvordan, [skal du se Oversigt over opdateringskanaler til Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).

- Beslut, om du vil anvende opdateringer automatisk fra internettet eller fra en lokal deling. Hvis du vil se hvordan, skal [du se Vælg, hvordan du administrerer opdateringer Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).

- Gennemgå Office Opdater Indstillinger at styre, hvordan opdateringer anvendes på slutbrugere:

    - [Konfigurer opdateringsindstillinger for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).
    - [Definer, hvordan Office opdateres, når den er installeret.](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Når du installerer Office-apps til flere brugere, skal du bruge værktøjet Office Customization til at opbygge konfigurationsfiler til installation og konfigurere Office-opdateringer ved hjælp af Office-udrulningsværktøjet. Du kan finde flere oplysninger [i Oversigt over Office-tilpasningsværktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) og [Office-udrulningsværktøjet.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

- Du kan finde et eksempel på, hvordan du konfigurerer brugergrupper til installation Office opdateringer, [under Installere Microsoft 365 Apps fra en lokal kilde.](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)
-   Overvej at bruge forceAppShutdown-indstillingen i tilfælde af Office opdateringer ikke anvendes til nogle få brugere på grund af åbne Office apps. Du kan finde flere oplysninger i [egenskaben FORCEAPPSHUTDOWN (en del af egenskabselementet).](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element) 

**Se også**

[Oversigt over opdateringsprocessen for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).  
[Udgive oplysninger om opdateringer til Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).  
[Administrer opdateringer til Microsoft 365 Apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).  
