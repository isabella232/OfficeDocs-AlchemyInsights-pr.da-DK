---
title: Anvend opdateringer til Office-Apps
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
ms.openlocfilehash: 8306d1acafe48f8779a8c02db8e3fe2f5d5f0e95
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716743"
---
# <a name="apply-updates-for-office-apps"></a>Anvend opdateringer til Office-Apps

Opdateringer til Office-Apps er som standard gratis, hentes automatisk og anvendes i baggrunden uden brugerinput. Hvis du vil køre opdateringer manuelt, hvis du kører i problemer med at anvende opdateringer, skal du se [Installer Office-opdateringer](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5). Hvis du vil have mere at vide, skal du se [fejlfinding af installation af Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).

Hvis du vil administrere Office-opdateringer til dine brugere, skal du overveje disse indstillinger:

- Vælg den rette Office-opdaterings kanal til din organisation ud fra den ønskede hyppighed af opdateringer. Se [Oversigt over opdaterings kanaler til Microsoft 365-apps for](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)at få mere at vide.

- Beslut, om du vil anvende opdateringer automatisk fra internettet eller fra et lokalt share. Du kan få mere at vide ved at se [vælge, hvordan du administrerer opdateringer til Microsoft 365-apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).

- Gennemgå indstillinger for Office Update for at styre, hvordan opdateringer anvendes på slutbruger computere:

    - [Konfigurer opdateringsindstillinger for Microsoft 365-apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).
    - [Definer, hvordan Office opdateres, efter det er installeret](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).

Når du installerer Office-Apps på flere brugere, kan du bruge Office-tilpasnings værktøjet til at opbygge konfigurationsfiler til installation og konfigurere Office-opdateringer ved hjælp af Office-udrulnings værktøjet. Se [Oversigt over Office-tilpasnings](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) værktøjet og [Office-udrulnings værktøjet](https://go.microsoft.com/fwlink/p/?LinkID=626065)for at få flere oplysninger.

- Hvis du vil have et eksempel på, hvordan du konfigurerer brugergrupper til installation af Office-opdateringer, skal du se [installere Microsoft 365-apps fra en lokal kilde](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).
-   Overvej at bruge indstillingen ForceAppShutdown i tilfælde af, at Office-opdateringer ikke bliver anvendt på nogle få brugere på grund af åbne Office-Apps. Du kan finde flere oplysninger i [egenskaben FORCEAPPSHUTDOWN (en del af egenskabselementet)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element). 

**Se også**

[Oversigt over opdateringsprocessen for Microsoft 365-apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).  
[Frigiv oplysninger om opdateringer til Microsoft 365-apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).  
[Administrer opdateringer til microsoft 365-apps med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).  
