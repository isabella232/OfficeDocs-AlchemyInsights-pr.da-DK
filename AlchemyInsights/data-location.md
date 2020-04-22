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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655276"
---
# <a name="data-location"></a><span data-ttu-id="4f298-102">Placering af data</span><span class="sxs-lookup"><span data-stu-id="4f298-102">Data location</span></span>

<span data-ttu-id="4f298-103">Du kan se placeringen af din lejer i Administration eller ved at oprette forbindelse til Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4f298-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="4f298-104">**Administration:**</span><span class="sxs-lookup"><span data-stu-id="4f298-104">**Admin center:**</span></span>
1. <span data-ttu-id="4f298-105">Log på [Administration](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="4f298-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="4f298-106">Vælg**Organisationsprofil** **for indstillinger** > .</span><span class="sxs-lookup"><span data-stu-id="4f298-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="4f298-107">Vælg **Vis detaljer**under **Dataplacering**.</span><span class="sxs-lookup"><span data-stu-id="4f298-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="4f298-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="4f298-108">**PowerShell:**</span></span>
1. <span data-ttu-id="4f298-109">Opret forbindelse til Exchange Online ved hjælp af Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4f298-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="4f298-110">Udfør [cmdlet'en Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for at få vist en liste over lejerens egenskaber.</span><span class="sxs-lookup"><span data-stu-id="4f298-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="4f298-111">Kig på OrganizationId ejendom.</span><span class="sxs-lookup"><span data-stu-id="4f298-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="4f298-112">Når du har dataplaceringen for EXO og SPO, kan du bestemme dataplaceringen for andre tjenester, du kan bruge fra [det sted, hvor dine data er placeret.](https://products.office.com/where-is-your-data-located)</span><span class="sxs-lookup"><span data-stu-id="4f298-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>