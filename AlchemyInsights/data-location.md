---
title: Placering af data
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627840"
---
# <a name="data-location"></a><span data-ttu-id="117b5-102">Placering af data</span><span class="sxs-lookup"><span data-stu-id="117b5-102">Data location</span></span>

<span data-ttu-id="117b5-103">Du kan få vist placeringen af din Office 365-lejer i administrationscenteret eller ved at oprette forbindelse til Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="117b5-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="117b5-104">**Admin Center:**</span><span class="sxs-lookup"><span data-stu-id="117b5-104">**Admin center:**</span></span>
1. <span data-ttu-id="117b5-105">Log på [Admin Center](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="117b5-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="117b5-106">Vælg **Indstillinger** > **organisations profil**.</span><span class="sxs-lookup"><span data-stu-id="117b5-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="117b5-107">Vælg **Vis detaljer**under **data placering**.</span><span class="sxs-lookup"><span data-stu-id="117b5-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="117b5-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="117b5-108">**PowerShell:**</span></span>
1. <span data-ttu-id="117b5-109">Opret forbindelse til Exchange Online ved hjælp af Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="117b5-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="117b5-110">Kør cmdlet'en [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for at få vist en liste over din lejer egenskaber.</span><span class="sxs-lookup"><span data-stu-id="117b5-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="117b5-111">Se på egenskaben OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="117b5-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="117b5-112">Når du har dataplaceringen for EXO og SPO, kan du bestemme dataplaceringen for andre tjenester, du kan bruge, fra [hvor dine data er placeret](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="117b5-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>