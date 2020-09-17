---
title: Opdater DNS-poster for at beholde dit websted hos din nuværende udbyder
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815779"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="93ff5-102">Opdater DNS-poster for at beholde dit websted hos din nuværende udbyder</span><span class="sxs-lookup"><span data-stu-id="93ff5-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="93ff5-103">I Microsoft 365 administration skal du gå til siden **konfigurations**  >  [domæner](https://admin.microsoft.com/Adminportal#/Domains) og vælge det domæne, du vil bruge til dit websted, på listen over domæner.</span><span class="sxs-lookup"><span data-stu-id="93ff5-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="93ff5-104">Vælg **+ ny brugerdefineret post** , og angiv følgende:</span><span class="sxs-lookup"><span data-stu-id="93ff5-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="93ff5-105">For **DNS-type** skal du skrive: **A (adresse)**</span><span class="sxs-lookup"><span data-stu-id="93ff5-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="93ff5-106">For **værtsnavn eller alias**skal du skrive følgende: **@**</span><span class="sxs-lookup"><span data-stu-id="93ff5-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="93ff5-107">For **IP-adresse**skal du skrive den statiske IP-adresse på dit websted, hvor den er hostet (f. eks. 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="93ff5-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="93ff5-108">Det skal være en  *statisk*  IP-adresse for webstedet, ikke en  *dynamisk*  IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="93ff5-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="93ff5-109">Kontrollér med det websted, hvor dit websted er hosted, for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.</span><span class="sxs-lookup"><span data-stu-id="93ff5-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="93ff5-110">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="93ff5-110">Select **Save**.</span></span>

<span data-ttu-id="93ff5-111">Derudover kan du oprette en CNAME-post for at hjælpe kunder med at finde dit websted.</span><span class="sxs-lookup"><span data-stu-id="93ff5-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="93ff5-112">Vælg **+ ny brugerdefineret post** , og angiv følgende:</span><span class="sxs-lookup"><span data-stu-id="93ff5-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="93ff5-113">For **DNS-type** skal du skrive: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="93ff5-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="93ff5-114">For **værtsnavn eller alias**skal du skrive følgende: **www**</span><span class="sxs-lookup"><span data-stu-id="93ff5-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="93ff5-115">For **Point to Address skal du**skrive det fulde domænenavn (FQDN) til dit websted (f. eks. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="93ff5-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="93ff5-116">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="93ff5-116">Select **Save**.</span></span>
