---
title: Opdatere DNS-poster for at beholde dit websted hos din nuværende hostingudbyder
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827506"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="53496-102">Opdatere DNS-poster for at beholde dit websted hos din nuværende hostingudbyder</span><span class="sxs-lookup"><span data-stu-id="53496-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="53496-103">I Microsoft 365 Administration skal du gå til siden **Konfiguration** af domæner og vælge det domæne, du bruger til dit websted, på  >  [](https://admin.microsoft.com/Adminportal#/Domains) listen over domæner.</span><span class="sxs-lookup"><span data-stu-id="53496-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="53496-104">Vælg **+ Ny brugerdefineret** post, og angiv følgende:</span><span class="sxs-lookup"><span data-stu-id="53496-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="53496-105">Til **DNS-type** skal du **skrive: A (adresse)**</span><span class="sxs-lookup"><span data-stu-id="53496-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="53496-106">For **Værtsnavn eller Alias** skal du skrive følgende: **@**</span><span class="sxs-lookup"><span data-stu-id="53496-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="53496-107">For **IP-adresse** skal du skrive den statiske IP-adresse til dit websted, hvor det aktuelt hostes (f.eks. 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="53496-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="53496-108">Dette skal være en  *statisk*  IP-adresse til webstedet, ikke en  *dynamisk*  IP-adresse.</span><span class="sxs-lookup"><span data-stu-id="53496-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="53496-109">Kontakt webstedet, hvor dit websted hostes, for at sikre, at du kan få en statisk IP-adresse til dit offentlige websted.</span><span class="sxs-lookup"><span data-stu-id="53496-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="53496-110">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="53496-110">Select **Save**.</span></span>

<span data-ttu-id="53496-111">Desuden kan du oprette en CNAME-post for at hjælpe kunderne med at finde dit websted.</span><span class="sxs-lookup"><span data-stu-id="53496-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="53496-112">Vælg **+ Ny brugerdefineret** post, og angiv følgende:</span><span class="sxs-lookup"><span data-stu-id="53496-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="53496-113">Til **DNS-type** skal du **angive: CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="53496-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="53496-114">For **Værtsnavn eller Alias** skal du skrive følgende: **www**</span><span class="sxs-lookup"><span data-stu-id="53496-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="53496-115">For **Peger på adresse** skal du skrive det fulde domænenavn for dit websted (f.eks. contoso.com).</span><span class="sxs-lookup"><span data-stu-id="53496-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="53496-116">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="53496-116">Select **Save**.</span></span>
