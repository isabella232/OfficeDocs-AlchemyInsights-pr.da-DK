---
title: Spørgsmål om, hvordan du bruger Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464313"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="9e806-102">Spørgsmål om, hvordan du bruger Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="9e806-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="9e806-103">Hent værktøjet Office installation fra [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="9e806-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="9e806-104">Når filen er hentet, ved at køre den selvudpakkende eksekverbare fil, der indeholder Office Deployment Tool eksekverbare (setup.exe) og en eksempelfil konfiguration (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="9e806-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="9e806-105">**At udelade eller fjerne Office 365 ProPlus produkter fra klientcomputere:**</span><span class="sxs-lookup"><span data-stu-id="9e806-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="9e806-p101">Når du installerer Office 365 ProPlus, kan du udelukke bestemte produkter. Følg disse trin for at installere Office med ODT gøres ved, men omfatter ExcludeApp elementet i konfigurationsfilen. For eksempel installerer denne konfigurationsfil Office 365 ProPlus produkter bortset fra Publisher:</span><span class="sxs-lookup"><span data-stu-id="9e806-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="9e806-109">Oversigt over Office Deployment Tool</span><span class="sxs-lookup"><span data-stu-id="9e806-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

