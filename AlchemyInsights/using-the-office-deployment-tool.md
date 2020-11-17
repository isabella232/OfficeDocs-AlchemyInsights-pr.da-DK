---
title: Brug af Office-udrulnings værktøjet
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085826"
---
# <a name="using-the-office-deployment-tool-odt"></a>Brug af Office udrulnings værktøj (ODT)

Du bruger Office udrulnings værktøj (ODT) til at installere Office 365-versioner af Office. Office udrulnings værktøj (setupodt.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes, når du installerer Office.
  
1. Hent den nyeste version af Office-udrulnings værktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Brug [Office-tilpasnings værktøjet (okt)](https://config.office.com) til at vælge dine installations præferencer og oprette XML-konfigurationsfilen. Eksportér konfigurationsfilen, og sæt den lokalt på den samme mappe, hvor setupodt.exe er placeret.

    **Bemærk:** Office-installationsproblemer opstår ofte på grund af forkert konfigurerede eller malformatted-konfigurationsfiler. For at undgå sådanne problemer anbefaler vi, at du bruger Office-tilpasnings værktøjet til at oprette konfigurationsfilen. Du kan også importere eksisterende konfigurationsfiler til Office-tilpasnings værktøjet.

3. Fra en kommandoprompt med administratorrettigheder skal du skifte til den placering, hvor setupodt.exe er placeret, og køre Office-udrulnings værktøjet i overførselstilstand og angive den konfigurationsfil, du lige har gemt. I dette eksempel hedder konfigurationsfilen Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Kør Office-udrulnings værktøjet i konfigurationstilstand, og Angiv konfigurationsfilen.

```setupodt.exe /configure Configuration.xml```

**Bemærk:** Du skal køre dette trin fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratorrettigheder på den computer.

Du kan få mere at vide om, hvordan du bruger Office-udrulnings værktøjet til dine Microsoft 365-apps til virksomheds installationsscenarier, under [Oversigt over Office-udrulnings værktøjet](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Du kan finde flere oplysninger om, hvordan du bruger Office-tilpasnings værktøjet, under [Oversigt over Office-tilpasnings værktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
