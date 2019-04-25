---
title: Spørgsmål om, hvordan du bruger Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371762"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørgsmål om, hvordan du bruger Office Deployment Tool (ODT)

Hent værktøjet Office installation fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når filen er hentet, ved at køre den selvudpakkende eksekverbare fil, der indeholder Office Deployment Tool eksekverbare (setup.exe) og en eksempelfil konfiguration (configuration.xml).
  
 **At udelade eller fjerne Office 365 ProPlus produkter fra klientcomputere:**
  
Når du installerer Office 365 ProPlus, kan du udelukke bestemte produkter. Følg disse trin for at installere Office med ODT gøres ved, men omfatter ExcludeApp elementet i konfigurationsfilen. For eksempel installerer denne konfigurationsfil Office 365 ProPlus produkter bortset fra Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversigt over Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

