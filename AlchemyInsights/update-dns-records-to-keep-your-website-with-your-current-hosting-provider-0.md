---
title: Opdatere DNS-poster for at holde dit websted hos din nuværende udbyder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665754"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="7b8e4-102">Opdatere DNS-poster for at holde dit websted hos din nuværende udbyder</span><span class="sxs-lookup"><span data-stu-id="7b8e4-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="7b8e4-103">I Microsoft 365 Administration skal **Setup**du gå til siden  >  [Installationsdomæner,](https://portal.office.com/adminportal/home#/Domains) og vælg det domæne, du bruger til dit websted, på listen over domæner.</span><span class="sxs-lookup"><span data-stu-id="7b8e4-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="7b8e4-104">Vælg **+ Ny brugerdefineret post,** og angiv følgende:</span><span class="sxs-lookup"><span data-stu-id="7b8e4-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="7b8e4-105">For **DNS-type** enter: **A (Adresse)**</span><span class="sxs-lookup"><span data-stu-id="7b8e4-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="7b8e4-106">Skriv følgende under **Værtsnavn eller Alias:\*\*\*\*@**</span><span class="sxs-lookup"><span data-stu-id="7b8e4-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="7b8e4-107">For **IP-adresse**skal du skrive den statiske IP-adresse for dit websted, hvor det aktuelt er hostet (f.eks. 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="7b8e4-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="7b8e4-108">Dette skal være en *statisk* IP-adresse til webstedet, ikke en *dynamisk* IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="7b8e4-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="7b8e4-109">Check med websted, hvor dit websted er hostet for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.</span><span class="sxs-lookup"><span data-stu-id="7b8e4-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="7b8e4-110">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="7b8e4-110">Select **Save**.</span></span>

<span data-ttu-id="7b8e4-111">Derudover kan du oprette en CNAME-post for at hjælpe kunderne med at finde dit websted.</span><span class="sxs-lookup"><span data-stu-id="7b8e4-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="7b8e4-112">Vælg **+ Ny brugerdefineret post,** og angiv følgende:</span><span class="sxs-lookup"><span data-stu-id="7b8e4-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="7b8e4-113">For **DNS-type** skal du indtaste: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="7b8e4-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="7b8e4-114">Skriv følgende under **Værtsnavn eller Alias:** **www:**</span><span class="sxs-lookup"><span data-stu-id="7b8e4-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="7b8e4-115">For **point til adresse**skal du skrive det fuldt kvalificerede domænenavn (FQDN) for dit websted (f.eks. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7b8e4-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="7b8e4-116">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="7b8e4-116">Select **Save**.</span></span>
