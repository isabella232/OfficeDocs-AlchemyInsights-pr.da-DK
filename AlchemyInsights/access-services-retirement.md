---
title: Adgang tjenester pensionering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687252"
---
# <a name="access-services-retirement"></a><span data-ttu-id="60b58-102">Adgang tjenester pensionering</span><span class="sxs-lookup"><span data-stu-id="60b58-102">Access services retirement</span></span>

<span data-ttu-id="60b58-103">Som vi oprindeligt annonceret i MC97576, i marts 2017, og fortsatte med at kommunikere i det forløbne år Access Services bliver pensioneret.</span><span class="sxs-lookup"><span data-stu-id="60b58-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="60b58-104">Den næste fase i denne proces vil være fjernelse af Access Web-databaser, der bruger SharePoint lister som deres underliggende datalagring.</span><span class="sxs-lookup"><span data-stu-id="60b58-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="60b58-105">**Hvordan påvirker det mig?**</span><span class="sxs-lookup"><span data-stu-id="60b58-105">**How does this affect me?**</span></span>

<span data-ttu-id="60b58-106">Fra juni 2019 stopper vi oprettelsen af nye Access-databaser i SharePoint Online og lukker tjenesten og eventuelle resterende apps inden april 2020.</span><span class="sxs-lookup"><span data-stu-id="60b58-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="60b58-107">**Hvad skal jeg gøre for at forberede mig på denne ændring?**</span><span class="sxs-lookup"><span data-stu-id="60b58-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="60b58-108">Vi opfordrer dig til at oprette en overgangsplan for organisationens Access-webdatabaser.</span><span class="sxs-lookup"><span data-stu-id="60b58-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="60b58-109">Administratorer kan bruge [SharePoint Access-appscanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at få en oversigt over de Access-apps, som websteder bruger.</span><span class="sxs-lookup"><span data-stu-id="60b58-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="60b58-110">Du kan overføre Data til Access-webdatabaser på flere måder:</span><span class="sxs-lookup"><span data-stu-id="60b58-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="60b58-111">Import til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="60b58-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="60b58-112">Vi anbefaler også, at du udforsker Microsoft PowerApps som en alternativ platform til at oprette forretningsløsninger uden kode til web- og mobilenheder.</span><span class="sxs-lookup"><span data-stu-id="60b58-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>