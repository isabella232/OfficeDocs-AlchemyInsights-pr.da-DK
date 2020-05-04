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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="0b8f5-102">Spørgsmål om, hvordan ODT (Office Deployment Tool) bruges</span><span class="sxs-lookup"><span data-stu-id="0b8f5-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="0b8f5-103">Hent Office-installationsværktøjet fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="0b8f5-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="0b8f5-104">Når du har hentet filen, skal du køre den selvudpakkende eksekverbare fil, som indeholder eksekverbar Office Deployment Tool (setup.exe) og en eksempelkonfigurationsfil (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="0b8f5-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="0b8f5-105">**Sådan udelukkes eller fjernes Microsoft 365 Apps til virksomhedsprodukter fra klientcomputere:**</span><span class="sxs-lookup"><span data-stu-id="0b8f5-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="0b8f5-106">Når du installerer Microsoft 365 Apps til virksomheder, kan du ekskludere bestemte produkter.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="0b8f5-107">Det kan du gøre ved at følge trinnene til installation af Office med ODT, men inkludere elementet ExcludeApp i konfigurationsfilen.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="0b8f5-108">Denne konfigurationsfil installerer f.eks.</span><span class="sxs-lookup"><span data-stu-id="0b8f5-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="0b8f5-109">Oversigt over Office-installationsværktøjet</span><span class="sxs-lookup"><span data-stu-id="0b8f5-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

