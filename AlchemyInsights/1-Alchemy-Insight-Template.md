---
title: 'samme som filnavn er bedst [regel #-beskrivelse]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634498"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="dc3e6-102">Påkrævede Alchemy hovedet H1, H2's virker ikke.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="dc3e6-103">Bedste fremgangsmåder og retningslinjer til oprettelse af Alchemy:</span><span class="sxs-lookup"><span data-stu-id="dc3e6-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="dc3e6-104">**Kan ikke sammensættes Alchemy indblik i mapper**- det ødelægges URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="dc3e6-105">Vi søger til at løse dette.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="dc3e6-106">Filerne i mappen **AlchemyInsights** skal have regel-ID og navn på regel fra [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="dc3e6-107">ex.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-107">ex.</span></span> <span data-ttu-id="dc3e6-108">***976-How-to-enable-litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="dc3e6-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="dc3e6-109">Brug metadataene i toppen af denne fil som skabelon.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="dc3e6-110">Intet andet er påkrævet.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-110">Nothing else is required.</span></span>
1. <span data-ttu-id="dc3e6-111">Gå til afsnittet i [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) **kunden indsigt titel:** og brug, der peger som en start til H1 titlen for indsigt.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="dc3e6-112">Alchemy viden skal have en enkelt H1 øverst eller de brydes i produktionen.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="dc3e6-113">H2s gengive ikke, så brug **fed** eller andre konventioner til at angive separate sektioner.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="dc3e6-114">Udfyld derefter brødtekst ved hjælp af udkast til materialet i afsnittet kunden indsigt i siden Alchemy regel</span><span class="sxs-lookup"><span data-stu-id="dc3e6-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="dc3e6-115">Punktopstillede lister er det fint</span><span class="sxs-lookup"><span data-stu-id="dc3e6-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="dc3e6-116">Nummererede lister for</span><span class="sxs-lookup"><span data-stu-id="dc3e6-116">Numbered lists too</span></span>
    1. <span data-ttu-id="dc3e6-117">**Fed** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="dc3e6-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="dc3e6-118">Links skal altid være en **"links til web" / eksterne** eller **deep-links til elementer i Brugergrænsefladen**, ikke interne hyperlinks.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="dc3e6-119">Og det er virkelig allerede lidt for langt.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-119">And this is really already a bit too long.</span></span> <span data-ttu-id="dc3e6-120">Den bedste fremgangsmåde er ca 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="dc3e6-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="dc3e6-121">Når indholdet er klar, kan du trække det til den levende gren.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="dc3e6-122">Derefter skal du gå til [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) og indtaste filnavnet i feltet URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="dc3e6-123">Kontroller, at indsigt, revideres og offentliggøres, siger "Ja", og klik derefter på Opdater regel.</span><span class="sxs-lookup"><span data-stu-id="dc3e6-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="dc3e6-124">**(Det ser pænere i den nye version af portalen - slippe hurtigt.)** 
 ![URL-felt](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="dc3e6-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

