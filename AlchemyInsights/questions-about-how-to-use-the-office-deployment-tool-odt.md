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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774885"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørgsmål om, hvordan du bruger Office udrulnings værktøj (ODT)

Hent Office-udrulnings værktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har downloadet filen, skal du køre den selvudpakkende eksekverbare fil, der indeholder Office-udrulnings værktøjet eksekverbar fil (setup.exe), og en eksempel konfigurations fil (configuration.xml).
  
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
  

