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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="6dfc9-102">Spørgsmål om, hvordan du bruger Office udrulnings værktøj (ODT)</span><span class="sxs-lookup"><span data-stu-id="6dfc9-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="6dfc9-103">Hent Office-udrulnings værktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="6dfc9-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="6dfc9-104">Når du har downloadet filen, skal du køre den selvudpakkende eksekverbare fil, der indeholder Office-udrulnings værktøjet eksekverbar fil (setupodt.exe), og en eksempel konfigurations fil (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="6dfc9-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="6dfc9-105">**Hvis du vil udelade eller fjerne Microsoft 365-apps til virksomheds produkter fra klientcomputere, skal du gøre følgende:**</span><span class="sxs-lookup"><span data-stu-id="6dfc9-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="6dfc9-106">Når du installerer Microsoft 365-apps til Enterprise, kan du udelukke bestemte produkter.</span><span class="sxs-lookup"><span data-stu-id="6dfc9-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="6dfc9-107">Hvis du vil gøre dette, skal du følge trinnene for at installere Office med ODT, men medtage ExcludeApp-elementet i konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="6dfc9-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="6dfc9-108">For eksempel installerer konfigurationsfilen alle Microsoft 365-apps til virksomheds produkter undtagen Publisher:</span><span class="sxs-lookup"><span data-stu-id="6dfc9-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="6dfc9-109">Oversigt over Office-udrulnings værktøjet</span><span class="sxs-lookup"><span data-stu-id="6dfc9-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

