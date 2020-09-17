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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="a9796-102">Spørgsmål om, hvordan du bruger Office udrulnings værktøj (ODT)</span><span class="sxs-lookup"><span data-stu-id="a9796-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a9796-103">Hent Office-udrulnings værktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a9796-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="a9796-104">Når du har downloadet filen, skal du køre den selvudpakkende eksekverbare fil, der indeholder Office-udrulnings værktøjet eksekverbar fil (setup.exe), og en eksempel konfigurations fil (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="a9796-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="a9796-105">**Hvis du vil udelade eller fjerne Microsoft 365-apps til virksomheds produkter fra klientcomputere, skal du gøre følgende:**</span><span class="sxs-lookup"><span data-stu-id="a9796-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="a9796-106">Når du installerer Microsoft 365-apps til Enterprise, kan du udelukke bestemte produkter.</span><span class="sxs-lookup"><span data-stu-id="a9796-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="a9796-107">Hvis du vil gøre dette, skal du følge trinnene for at installere Office med ODT, men medtage ExcludeApp-elementet i konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="a9796-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="a9796-108">For eksempel installerer konfigurationsfilen alle Microsoft 365-apps til virksomheds produkter undtagen Publisher:</span><span class="sxs-lookup"><span data-stu-id="a9796-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="a9796-109">Oversigt over Office-udrulnings værktøjet</span><span class="sxs-lookup"><span data-stu-id="a9796-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

