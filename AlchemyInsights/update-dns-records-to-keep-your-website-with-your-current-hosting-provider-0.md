---
title: Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
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
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925279"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="87582-102">Opdater DNS-poster for at beholde dit websted hos din nuværende hosting-udbyder</span><span class="sxs-lookup"><span data-stu-id="87582-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="87582-103">Vælg det domæne, du bruger til dit websted på listen over domæner, på siden [domæner](https://portal.office.com/adminportal/home#/Domains) .</span><span class="sxs-lookup"><span data-stu-id="87582-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="87582-104">Vælg **+ ny brugerdefineret post** , og Skriv følgende:</span><span class="sxs-lookup"><span data-stu-id="87582-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="87582-105">Angiv for **DNS-type** : **(adresse)**</span><span class="sxs-lookup"><span data-stu-id="87582-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="87582-106">For **Host-navn eller Alias**, skal du skrive følgende:**@**</span><span class="sxs-lookup"><span data-stu-id="87582-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="87582-107">Skriv den statiske IP-adresse på dit websted, hvor den aktuelt er placeret (f.eks, 172.16.140.1) til **IP-adresse**.</span><span class="sxs-lookup"><span data-stu-id="87582-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="87582-108">Det skal være en *statisk* IP-adresse for webstedet, ikke en *dynamisk* IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="87582-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="87582-109">Spørg websted, hvor webstedet er vært for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.</span><span class="sxs-lookup"><span data-stu-id="87582-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="87582-110">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="87582-110">Select **Save**.</span></span>

<span data-ttu-id="87582-111">Desuden kan du oprette en CNAME-post for at hjælpe kunderne med at finde dit websted.</span><span class="sxs-lookup"><span data-stu-id="87582-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="87582-112">Vælg **+ ny brugerdefineret post** , og Skriv følgende:</span><span class="sxs-lookup"><span data-stu-id="87582-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="87582-113">Angiv for **DNS-type** : **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="87582-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="87582-114">**Host-navn eller Alias**, skal du skrive følgende: **www**</span><span class="sxs-lookup"><span data-stu-id="87582-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="87582-115">Skriv det fuldt kvalificerede domænenavn (FQDN) på dit websted (for eksempel contoso.com) for **peger på adresse**.</span><span class="sxs-lookup"><span data-stu-id="87582-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="87582-116">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="87582-116">Select **Save**.</span></span>
