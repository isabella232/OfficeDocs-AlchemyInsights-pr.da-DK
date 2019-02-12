---
title: Ved hjælp af værktøjet Office installation
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29898640"
---
# <a name="using-the-office-deployment-tool-odt"></a>Ved hjælp af Office Deployment Tool (ODT)

Du kan bruge Office Deployment Tool (ODT) til at installere Office 365-versioner af Office. Værktøjet Office installation (setup.exe) køres fra kommandolinjen og bruger en XML-konfigurationsfil til at bestemme, hvilke indstillinger der skal anvendes, når du installerer Office.
  
1. Hent den nyeste version af værktøjet Office installation fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Brug [Office Customization Tool (OCT)](https://config.office.com) til at vælge dine indstillinger for installation og oprette XML-konfigurationsfilen. Eksportere konfigurationsfilen, og Placer den lokalt på den samme mappe, hvor setup.exe er placeret. 
    
    **Bemærk:** Office-installation, der ofte opstår problemer forfalder til forkert konfigureret eller malformatted konfigurationsfiler. For at undgå sådanne problemer, anbefaler vi, at du bruger Office Customization Tool til at oprette konfigurationsfilen. Du kan også importere eksisterende konfigurationsfiler til Office-tilpasningsværktøjet. 
    
3. Skift til den placering, hvor setup.exe er placeret fra en kommandoprompt og køre værktøjet Office installation i download-tilstand, og Angiv den konfigurationsfil, du lige har gemt. I dette eksempel hedder konfigurationsfilen Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Kør værktøjet Office installation i konfigurere tilstand og angive konfigurationsfilen.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Bemærk:** Fra den klientcomputer, hvor du vil installere Office, og du skal have lokale administratorrettigheder på denne computer, skal du udføre dette trin. 
    
Hvis du vil vide mere om brugen af Office Deployment Tool for Office 365 ProPlus installationsscenarier, se [Oversigt over værktøjet Office installation](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Du kan finde flere oplysninger om, hvordan du bruger Office-tilpasningsværktøjet, [Oversigt over Office-tilpasningsværktøjet](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

