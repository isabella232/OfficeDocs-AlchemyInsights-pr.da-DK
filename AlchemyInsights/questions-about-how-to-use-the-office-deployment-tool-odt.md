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
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553534"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørgsmål om, hvordan du bruger Office Deployment Tool (ODT)

Hent Office-installationsværktøjet fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har hentet filen, skal du køre den selvudpakkende eksekverbare fil, som indeholder den eksekverbare Office-installationsværktøj (setup. exe) og en eksempel konfigurations fil (Configuration. XML).
  
 **Sådan udelukker eller fjerner du Office 365 ProPlus-produkter fra klientcomputere:**
  
Når du installerer Office 365 ProPlus, kan du udelukke bestemte produkter. Det kan du gøre ved at følge trinnene til installation af Office med ODT, men du kan inkludere elementet ExcludeApp i konfigurationsfilen. For eksempel installerer denne konfigurationsfil alle Office 365 ProPlus-produkter undtagen Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversigt over Office-installationsværktøjet](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

