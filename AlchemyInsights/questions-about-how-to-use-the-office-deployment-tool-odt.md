---
title: Spørgsmål om, hvordan du bruger Office udrulnings værktøj (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086150"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørgsmål om, hvordan du bruger Office udrulnings værktøj (ODT)

Hent Office-udrulnings værktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har downloadet filen, skal du køre den selvudpakkende eksekverbare fil, der indeholder Office-udrulnings værktøjet eksekverbar fil (setupodt.exe), og en eksempel konfigurations fil (configuration.xml).
  
 **Hvis du vil udelade eller fjerne Microsoft 365-apps til virksomheds produkter fra klientcomputere, skal du gøre følgende:**
  
Når du installerer Microsoft 365-apps til Enterprise, kan du udelukke bestemte produkter. Hvis du vil gøre dette, skal du følge trinnene for at installere Office med ODT, men medtage ExcludeApp-elementet i konfigurationsfilen. For eksempel installerer konfigurationsfilen alle Microsoft 365-apps til virksomheds produkter undtagen Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversigt over Office-udrulnings værktøjet](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

