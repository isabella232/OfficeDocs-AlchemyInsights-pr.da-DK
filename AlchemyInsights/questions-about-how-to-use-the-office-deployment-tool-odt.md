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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="1f921-102">Spørgsmål om, hvordan du bruger Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="1f921-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="1f921-103">Hent Office-installationsværktøjet fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="1f921-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="1f921-104">Når du har hentet filen, skal du køre den selvudpakkende eksekverbare fil, som indeholder den eksekverbare Office-installationsværktøj (setup. exe) og en eksempel konfigurations fil (Configuration. XML).</span><span class="sxs-lookup"><span data-stu-id="1f921-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="1f921-105">**Sådan udelukker eller fjerner du Office 365 ProPlus-produkter fra klientcomputere:**</span><span class="sxs-lookup"><span data-stu-id="1f921-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="1f921-106">Når du installerer Office 365 ProPlus, kan du udelukke bestemte produkter.</span><span class="sxs-lookup"><span data-stu-id="1f921-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="1f921-107">Det kan du gøre ved at følge trinnene til installation af Office med ODT, men du kan inkludere elementet ExcludeApp i konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="1f921-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="1f921-108">For eksempel installerer denne konfigurationsfil alle Office 365 ProPlus-produkter undtagen Publisher:</span><span class="sxs-lookup"><span data-stu-id="1f921-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="1f921-109">Oversigt over Office-installationsværktøjet</span><span class="sxs-lookup"><span data-stu-id="1f921-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

