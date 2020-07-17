---
title: samme som filnavn er bedst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750964"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="82c5a-102">"Krævede Alkymi Header H1, H2's virker ikke."</span><span class="sxs-lookup"><span data-stu-id="82c5a-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="82c5a-103">Bedste fremgangsmåder og retningslinjer for alkymi authoring:</span><span class="sxs-lookup"><span data-stu-id="82c5a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="82c5a-104">**Må ikke indlejre Alchemy Insights i mapper**- dette vil bryde url struktur.</span><span class="sxs-lookup"><span data-stu-id="82c5a-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="82c5a-105">Vi undersøger, om vi skal ordne det her.</span><span class="sxs-lookup"><span data-stu-id="82c5a-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="82c5a-106">Filer i mappen **AlchemyInsights** skal have filnavne med små bogstaver med bindestreger til mellemrum ex.</span><span class="sxs-lookup"><span data-stu-id="82c5a-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="82c5a-107">***hvordan-til-aktivere-retssager-hold***.</span><span class="sxs-lookup"><span data-stu-id="82c5a-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="82c5a-108">Medtag regel-id'et eller bucket-id'et fra [alkymipartnerportalen](https://alchemyportal.azurewebsites.net) i ms.custom-feltet.</span><span class="sxs-lookup"><span data-stu-id="82c5a-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="82c5a-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="82c5a-109">ex.</span></span> <span data-ttu-id="82c5a-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="82c5a-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="82c5a-111">Brug resten af metadataene øverst i denne fil som skabelon.</span><span class="sxs-lookup"><span data-stu-id="82c5a-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="82c5a-112">På [Alchemy Partner-portalen skal](https://alchemyportal.azurewebsites.net)du navigere ned til afsnittet **Customer Insight Title:** og bruge det som udgangspunkt for din H1-titel til indsigten.</span><span class="sxs-lookup"><span data-stu-id="82c5a-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="82c5a-113">Alkymi Insights SKAL kun have en enkelt H1 i toppen, eller de vil bryde i produktionen.</span><span class="sxs-lookup"><span data-stu-id="82c5a-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="82c5a-114">H2s ikke gøre enten så brug **fed** eller andre konventioner til at betyde separate sektioner.</span><span class="sxs-lookup"><span data-stu-id="82c5a-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="82c5a-115">Udfyld derefter brødteksten ved hjælp af kladdematerialet i afsnittet Kundeindsigt på siden Alchemy Rule</span><span class="sxs-lookup"><span data-stu-id="82c5a-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="82c5a-116">Punktopstillinger er fine</span><span class="sxs-lookup"><span data-stu-id="82c5a-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="82c5a-117">Også opstilling af tal/bogstaver</span><span class="sxs-lookup"><span data-stu-id="82c5a-117">Numbered lists too</span></span>
    1. <span data-ttu-id="82c5a-118">**Fed** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="82c5a-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="82c5a-119">Links bør altid være enten **"links til web"/eksterne** eller **dybe links til UI elementer,** ikke interne links.</span><span class="sxs-lookup"><span data-stu-id="82c5a-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="82c5a-120">Billeder er ikke officielt understøttet på nuværende tidspunkt, men det er på køreplanen.</span><span class="sxs-lookup"><span data-stu-id="82c5a-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="82c5a-121">Og det er virkelig allerede lidt for længe.</span><span class="sxs-lookup"><span data-stu-id="82c5a-121">And this is really already a bit too long.</span></span> <span data-ttu-id="82c5a-122">Bedste praksis er omkring 400 tegn ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="82c5a-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="82c5a-123">Når dit indhold er klar, skal du trække det til live grenen.</span><span class="sxs-lookup"><span data-stu-id="82c5a-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="82c5a-124">Gå derefter til [Alchemy Partner-portalen,](https://alchemyportal.azurewebsites.net) og indtast filnavnet i url-feltet.</span><span class="sxs-lookup"><span data-stu-id="82c5a-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 