---
title: samme som filnavn er bedst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800039"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="c9ae1-102">Påkrævet Alchemy header H1, H2's dont arbejde.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="c9ae1-103">Bedste fremgangsmåder og retningslinjer for Alchemy authoring:</span><span class="sxs-lookup"><span data-stu-id="c9ae1-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="c9ae1-104">**Du må ikke indlejre Alchemy Insights i mapper**-dette vil bryde URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="c9ae1-105">Vi kigger på at ordne det her.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="c9ae1-106">Filer i mappen **Alchemyinsights** skal have små filnavne med bindestreger til mellemrum ex.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="c9ae1-107">***Sådan gør du-aktiver-retssager-hold***.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="c9ae1-108">Medtag regel-id'et eller bucket-id'et fra [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net) i MS. Custom-feltet.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="c9ae1-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-109">ex.</span></span> <span data-ttu-id="c9ae1-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="c9ae1-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="c9ae1-111">Brug resten af metadataene øverst i denne fil som skabelon.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="c9ae1-112">I [Alchemy partner portalen](https://alchemyportal.azurewebsites.net)skal du navigere ned til afsnittet **kunde Insight-titel:** og bruge det som udgangspunkt for din H1-titel til indsigten.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="c9ae1-113">Alchemy Insights skal kun have en enkelt H1 i toppen, eller de vil bryde i produktionen.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="c9ae1-114">H2S Render ikke enten så brug **fed** eller andre konventioner til at betyde separate sektioner.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="c9ae1-115">Udfyld derefter brødteksten ved hjælp af kladde materialet i afsnittet Kundeindsigt på siden Alchemy Rule</span><span class="sxs-lookup"><span data-stu-id="c9ae1-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="c9ae1-116">Punktopstillinger er fine</span><span class="sxs-lookup"><span data-stu-id="c9ae1-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="c9ae1-117">Nummererede lister også</span><span class="sxs-lookup"><span data-stu-id="c9ae1-117">Numbered lists too</span></span>
    1. <span data-ttu-id="c9ae1-118">**Fed** og *kursiv* er a-OK</span><span class="sxs-lookup"><span data-stu-id="c9ae1-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="c9ae1-119">Links skal altid være enten **"links til web"/eksterne** eller **dybe-links til UI elementer**, ikke interne links.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="c9ae1-120">Billeder er ikke officielt understøttet på dette tidspunkt, men det er på køreplanen.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="c9ae1-121">Og det er virkelig allerede lidt for længe.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-121">And this is really already a bit too long.</span></span> <span data-ttu-id="c9ae1-122">Bedste praksis er omkring 400 tegn---------------------------------</span><span class="sxs-lookup"><span data-stu-id="c9ae1-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="c9ae1-123">Når dit indhold er klar, skal du trække det til live grenen.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="c9ae1-124">Gå derefter til [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net) , og Indtast filnavnet i URL-feltet.</span><span class="sxs-lookup"><span data-stu-id="c9ae1-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 