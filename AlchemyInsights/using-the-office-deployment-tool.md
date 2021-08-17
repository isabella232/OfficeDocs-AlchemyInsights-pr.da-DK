---
title: Brug af Office til udrulning
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083764"
---
# <a name="using-the-office-deployment-tool-odt"></a>Brug af Office (ODT)

Du kan bruge Office (ODT) til at installere Office 365 versioner af Office. Installationsværktøjet Office (setup.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes, når du Office.
  
1. Download den nyeste version af Office fra [Microsoft Download Center.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Brug [OKT Office (Customization Tool) til at vælge](https://config.office.com) installationsindstillinger og oprette XML-konfigurationsfilen. Eksportér konfigurationsfilen, og placer den lokalt i den samme mappe, setup.exe er placeret.

    **Bemærk:** Office ofte opstår på grund af forkert konfigurerede eller forkert formaterede konfigurationsfiler. For at undgå sådanne problemer anbefaler vi, at du bruger Office til at oprette konfigurationsfilen. Du kan også importere eksisterende konfigurationsfiler til Office-tilpasningsværktøjet.

3. Fra en kommandoprompt med administrator administrator skal du skifte til den placering, hvor setup.exe er placeret, og køre Office-udrulningsværktøjet i downloadtilstand og angive den konfigurationsfil, du lige har gemt. I dette eksempel kaldes konfigurationsfilen Configuration.xml:

```setup.exe /download Configuration.xml```

4.Kør Office i konfigurationstilstand, og angiv konfigurationsfilen.

```setup.exe /configure Configuration.xml```

**Bemærk!** Du skal køre dette trin fra den klientcomputer, hvor du vil installere Office og du skal have lokale administratorrettigheder på computeren.

Du kan få mere at vide Office at bruge udrulningsværktøjet Microsoft 365 Apps for enterprise dine Microsoft 365 Apps for enterprise i Oversigt [over Office-udrulningsværktøj.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Du kan finde flere oplysninger om, hvordan du Office værktøjet til tilpasning af Office [oversigt over tilpasningsværktøjet.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
