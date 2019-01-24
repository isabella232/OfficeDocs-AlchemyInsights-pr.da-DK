---
title: Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464116"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="ecf75-102">Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder</span><span class="sxs-lookup"><span data-stu-id="ecf75-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="ecf75-103">Vælg det domæne, du bruger til dit websted, og vælg derefter **DNS-indstillingerne** i ruden management på listen over domæner, på siden [domæner](https://portal.office.com/adminportal/home#/Domains) .</span><span class="sxs-lookup"><span data-stu-id="ecf75-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="ecf75-104">Vælg **+ ny brugerdefineret post** , og Skriv følgende:</span><span class="sxs-lookup"><span data-stu-id="ecf75-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="ecf75-105">Angiv for **DNS-type** : **(adresse)**</span><span class="sxs-lookup"><span data-stu-id="ecf75-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="ecf75-106">For **Host-navn eller Alias**, skal du skrive følgende:**@**</span><span class="sxs-lookup"><span data-stu-id="ecf75-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="ecf75-107">Skriv den statiske IP-adresse på dit websted, hvor den aktuelt er placeret (f.eks, 172.16.140.1) til **IP-adresse**.</span><span class="sxs-lookup"><span data-stu-id="ecf75-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="ecf75-p101">Det skal være en *statisk* IP-adresse for webstedet, ikke en *dynamisk* IP-adresse. Spørg websted, hvor webstedet er vært for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.</span><span class="sxs-lookup"><span data-stu-id="ecf75-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="ecf75-110">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="ecf75-110">Select **Save**.</span></span> 
    
<span data-ttu-id="ecf75-111">Desuden kan du oprette en CNAME-post for at hjælpe kunderne med at finde dit websted.</span><span class="sxs-lookup"><span data-stu-id="ecf75-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="ecf75-112">Vælg **+ ny brugerdefineret post** , og Skriv følgende:</span><span class="sxs-lookup"><span data-stu-id="ecf75-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="ecf75-113">Angiv for **DNS-type** : **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="ecf75-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="ecf75-114">**Host-navn eller Alias**, skal du skrive følgende: **www**</span><span class="sxs-lookup"><span data-stu-id="ecf75-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="ecf75-115">Skriv det fuldt kvalificerede domænenavn (FQDN) på dit websted (for eksempel contoso.com) for **peger på adresse**.</span><span class="sxs-lookup"><span data-stu-id="ecf75-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="ecf75-116">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="ecf75-116">Select **Save**.</span></span> 
    

