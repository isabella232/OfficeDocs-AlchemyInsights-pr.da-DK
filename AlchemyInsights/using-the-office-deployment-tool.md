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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794905"
---
# <a name="using-the-office-deployment-tool-odt"></a>Brug af Office udrulnings værktøj (ODT)

Du bruger Office udrulnings værktøj (ODT) til at installere Office 365-versioner af Office. Office udrulnings værktøj (setup.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes, når du installerer Office.
  
1. Hent den nyeste version af Office-udrulnings værktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Brug [Office-tilpasnings værktøjet (okt)](https://config.office.com) til at vælge dine installations præferencer og oprette XML-konfigurationsfilen. Eksportér konfigurationsfilen, og sæt den lokalt på den samme mappe, hvor setup.exe er placeret.

    **Bemærk:** Office-installationsproblemer opstår ofte på grund af forkert konfigurerede eller malformatted-konfigurationsfiler. For at undgå sådanne problemer anbefaler vi, at du bruger Office-tilpasnings værktøjet til at oprette konfigurationsfilen. Du kan også importere eksisterende konfigurationsfiler til Office-tilpasnings værktøjet.

3. Fra en kommandoprompt med administratorrettigheder skal du skifte til den placering, hvor setup.exe er placeret, og køre Office-udrulnings værktøjet i overførselstilstand og angive den konfigurationsfil, du lige har gemt. I dette eksempel hedder konfigurationsfilen Configuration.xml:

```setup.exe /download Configuration.xml```

4. Kør Office-udrulnings værktøjet i konfigurationstilstand, og Angiv konfigurationsfilen.

```setup.exe /configure Configuration.xml```

**Bemærk:** Du skal køre dette trin fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratorrettigheder på den computer.

Du kan få mere at vide om, hvordan du bruger Office-udrulnings værktøjet til dine Microsoft 365-apps til virksomheds installationsscenarier, under [Oversigt over Office-udrulnings værktøjet](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Du kan finde flere oplysninger om, hvordan du bruger Office-tilpasnings værktøjet, under [Oversigt over Office-tilpasnings værktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
