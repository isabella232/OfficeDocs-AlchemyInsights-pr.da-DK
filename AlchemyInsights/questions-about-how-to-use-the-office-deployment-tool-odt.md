---
title: Spørgsmål om, hvordan du bruger Office -udrulningsværktøj (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959677"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørgsmål om, hvordan du bruger Office -udrulningsværktøj (ODT)

Download Office fra [Microsoft Download Center.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Når du har hentet filen, skal du køre den selvudpakkende eksekverbare fil, der indeholder den eksekverbare Office-udrulningsværktøj (setup.exe) og en eksempelkonfigurationsfil (configuration.xml).
  
 **For at udelukke eller fjerne Microsoft 365 Apps for enterprise fra klientcomputere:**
  
Når du installerer Microsoft 365 Apps for enterprise, kan du udelade bestemte produkter. Det gør du ved at følge trinnene for installation Office ODT, men medtag elementet ExcludeApp i din konfigurationsfil. Denne konfigurationsfil installerer f.eks. alle Microsoft 365 Apps for enterprise undtagen Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversigt over Office over udrulningsværktøjet](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

