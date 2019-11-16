---
title: Adgangstjenester pensionering
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747778"
---
# <a name="access-services-retirement"></a><span data-ttu-id="60e3e-102">Adgangstjenester pensionering</span><span class="sxs-lookup"><span data-stu-id="60e3e-102">Access services retirement</span></span>

<span data-ttu-id="60e3e-103">Som vi oprindeligt annonceret i MC97576, i marts 2017, og fortsatte med at kommunikere i løbet af det seneste år adgangstjenester er ved at blive pensioneret fra Office 365.</span><span class="sxs-lookup"><span data-stu-id="60e3e-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="60e3e-104">Den næste fase i denne proces vil være fjernelsen af Access-webdatabaser, der bruger SharePoint-lister som deres underliggende datalager.</span><span class="sxs-lookup"><span data-stu-id="60e3e-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="60e3e-105">**Hvordan påvirker det mig?**</span><span class="sxs-lookup"><span data-stu-id="60e3e-105">**How does this affect me?**</span></span>

<span data-ttu-id="60e3e-106">Fra og med juni 2019 vil vi stoppe oprettelsen af nye Access-databaser i SharePoint Online og lukke tjenesten og eventuelle resterende apps senest i april 2020.</span><span class="sxs-lookup"><span data-stu-id="60e3e-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="60e3e-107">**Hvad skal jeg gøre for at forberede mig på denne ændring?**</span><span class="sxs-lookup"><span data-stu-id="60e3e-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="60e3e-108">Vi opfordrer dig til at oprette en overgangsplan for organisationens Access-webdatabaser.</span><span class="sxs-lookup"><span data-stu-id="60e3e-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="60e3e-109">Administratorer kan bruge [SharePoint Access-appscanneren](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) til at hente en oversigt med de Access-apps, som websteder bruger.</span><span class="sxs-lookup"><span data-stu-id="60e3e-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="60e3e-110">Der er flere måder at migrere Access web databases data:</span><span class="sxs-lookup"><span data-stu-id="60e3e-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="60e3e-111">Importerer til en lokal Access-database (. ACCDB) eller til en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="60e3e-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="60e3e-112">Vi anbefaler også, at du udforsker Microsoft PowerApps som en alternativ platform til at oprette forretningsløsninger uden kode til web-og mobilenheder.</span><span class="sxs-lookup"><span data-stu-id="60e3e-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>