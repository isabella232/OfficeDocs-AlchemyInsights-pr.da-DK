---
title: Spørgsmål om, hvordan ODT (Office Deployment Tool) bruges
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010726"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Spørgsmål om, hvordan ODT (Office Deployment Tool) bruges

Hent Office-installationsværktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Når du har hentet filen, skal du køre den selvudpakkende eksekverbare fil, som indeholder eksekverbar Office Deployment Tool (setup.exe) og en eksempelkonfigurationsfil (configuration.xml).
  
 **Sådan udelukkes eller fjernes Microsoft 365 Apps til virksomhedsprodukter fra klientcomputere:**
  
Når du installerer Microsoft 365 Apps til virksomheder, kan du ekskludere bestemte produkter. Det kan du gøre ved at følge trinnene til installation af Office med ODT, men inkludere elementet ExcludeApp i konfigurationsfilen. Denne konfigurationsfil installerer f.eks.
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Oversigt over Office-installationsværktøjet](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

