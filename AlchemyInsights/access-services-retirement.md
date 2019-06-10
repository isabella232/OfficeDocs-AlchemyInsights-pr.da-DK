---
title: Access services-pension
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769431"
---
# <a name="access-services-retirement"></a><span data-ttu-id="72a3c-102">Access services-pension</span><span class="sxs-lookup"><span data-stu-id="72a3c-102">Access services retirement</span></span>

<span data-ttu-id="72a3c-103">Da vi oprindeligt blev offentliggjort i MC97576, i marts 2017 og fortsatte med at kommunikere over det seneste år er Access Services bliver afbrudt fra Office 365.</span><span class="sxs-lookup"><span data-stu-id="72a3c-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="72a3c-104">Den næste fase i denne proces vil være fjernelse af Web Access-databaser, der bruger SharePoint-lister som deres underliggende datalager.</span><span class="sxs-lookup"><span data-stu-id="72a3c-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="72a3c-105">**Hvordan påvirker det mig?**</span><span class="sxs-lookup"><span data-stu-id="72a3c-105">**How does this affect me?**</span></span>

<span data-ttu-id="72a3c-106">Start juni 2019, vi stopper oprettelsen af nye Access-databaser i SharePoint Online og lukke tjenesten og eventuelle resterende apps ved April 2020.</span><span class="sxs-lookup"><span data-stu-id="72a3c-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="72a3c-107">**Hvad skal jeg gøre for at forberede denne ændring?**</span><span class="sxs-lookup"><span data-stu-id="72a3c-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="72a3c-108">Vi opfordrer dig til at oprette en plan for overgangen til organisationens Access web-databaser.</span><span class="sxs-lookup"><span data-stu-id="72a3c-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="72a3c-109">Administratorer kan bruge [SharePoint adgang app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at få en oversigt over Access-programmer, websteder bruger.</span><span class="sxs-lookup"><span data-stu-id="72a3c-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="72a3c-110">Der er flere måder at overføre data fra Access web databaser:</span><span class="sxs-lookup"><span data-stu-id="72a3c-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="72a3c-111">Import til en lokal database i Access (. ACCDB) eller en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="72a3c-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="72a3c-112">Vi anbefaler også, at udforske Microsoft PowerApps som en alternativ platform til at oprette uden kode forretningsløsninger til web og mobile enheder.</span><span class="sxs-lookup"><span data-stu-id="72a3c-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>