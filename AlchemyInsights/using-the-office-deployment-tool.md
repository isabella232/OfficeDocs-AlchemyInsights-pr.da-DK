---
title: Brug af Office-installationsværktøjet
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010851"
---
# <a name="using-the-office-deployment-tool-odt"></a>Bruge ODT (Office Deployment Tool)

Du kan bruge ODT (Office Deployment Tool) til at installere Office 365-versioner af Office. Office Deployment Tool (setup.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes ved installation af Office.
  
1. Hent den nyeste version af Office Deployment Tool fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Brug [OKT (Office Customization Tool)](https://config.office.com) til at vælge installationsindstillingerne og oprette XML-konfigurationsfilen. Eksporter konfigurationsfilen, og placer den lokalt i den samme mappe, hvor setup.exe er placeret.

    **Bemærk:** Problemer med Office-installation opstår ofte på grund af forkert konfigurerede eller forkert formaterede konfigurationsfiler. Hvis du vil undgå sådanne problemer, anbefales det, at du bruger Office-tilpasningsværktøjet til at oprette konfigurationsfilen. Du kan også importere eksisterende konfigurationsfiler til Office-tilpasningsværktøjet.

3. Fra en kommandoprompt med en forhøjet kommando skal du skifte til den placering, hvor setup.exe er placeret, og køre Office-installationsværktøjet i overførselstilstand og angive den konfigurationsfil, du lige har gemt. I dette eksempel hedder konfigurationsfilen Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Kør Office-installationsværktøjet i konfigureretilstand, og angiv konfigurationsfilen.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Bemærk:** Du skal køre dette trin fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratortilladelser på den pågældende computer.

Hvis du vil have mere at vide om at bruge Office Deployment Tool til dine Microsoft 365 Apps til virksomhedsinstallationsscenarier, skal du se [Oversigt over Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Yderligere oplysninger om, hvordan du bruger Office-tilpasningsværktøjet, finder [du i Oversigt over Office-tilpasningsværktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
