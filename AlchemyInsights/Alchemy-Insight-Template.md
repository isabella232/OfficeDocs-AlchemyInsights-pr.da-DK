---
title: det samme som filnavnet er bedst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664128"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="36728-102">"Påkrævet Alchemy-sidehoved H1, H2's virker ikke."</span><span class="sxs-lookup"><span data-stu-id="36728-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="36728-103">Bedste fremgangsmåder og retningslinjer for Alchemy-redigering:</span><span class="sxs-lookup"><span data-stu-id="36728-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="36728-104">**Du må ikke indlejre Alchemy-indsigt i mapper**– dette bryder URL-strukturen ud.</span><span class="sxs-lookup"><span data-stu-id="36728-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="36728-105">Vi er ved at rette dette.</span><span class="sxs-lookup"><span data-stu-id="36728-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="36728-106">Filer i mappen **AlchemyInsights** skal have små filnavne med bindestreger for mellemrum.</span><span class="sxs-lookup"><span data-stu-id="36728-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="36728-107">***Sådan aktiverer du en retssag***.</span><span class="sxs-lookup"><span data-stu-id="36728-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="36728-108">Medtag regel-ID eller Bucket-ID fra [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net) i MS. brugerdefineret felt.</span><span class="sxs-lookup"><span data-stu-id="36728-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="36728-109">udvidet.</span><span class="sxs-lookup"><span data-stu-id="36728-109">ex.</span></span> <span data-ttu-id="36728-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="36728-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="36728-111">Brug resten af metadataene øverst i denne fil som skabelon.</span><span class="sxs-lookup"><span data-stu-id="36728-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="36728-112">I [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net)skal du gå til afsnittet **kundens indblikings titel:** og bruge det som udgangspunkt for din H1-titel for indsigt.</span><span class="sxs-lookup"><span data-stu-id="36728-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="36728-113">Alchemy indsigt må kun have et enkelt H1 øverst, eller de vil bryde op i produktion.</span><span class="sxs-lookup"><span data-stu-id="36728-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="36728-114">H2S gengives ikke, så brug af **fed** eller andre konventioner til at angive separate sektioner.</span><span class="sxs-lookup"><span data-stu-id="36728-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="36728-115">Derefter skal du udfylde brødteksten ved hjælp af kladde materialet i sektionen kunde indsigt på Alchemy-regel siden</span><span class="sxs-lookup"><span data-stu-id="36728-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="36728-116">Punktopstillinger er fine</span><span class="sxs-lookup"><span data-stu-id="36728-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="36728-117">Nummererede lister</span><span class="sxs-lookup"><span data-stu-id="36728-117">Numbered lists too</span></span>
    1. <span data-ttu-id="36728-118">**Fed** og *kursiv* er en-OK</span><span class="sxs-lookup"><span data-stu-id="36728-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="36728-119">Links bør altid være **"links til internettet"-/External** eller **dyb links til brugergrænsefladeelementer**, ikke interne kæder.</span><span class="sxs-lookup"><span data-stu-id="36728-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="36728-120">Billeder er ikke officielt understøttet på nuværende tidspunkt, men det er på køreplanen.</span><span class="sxs-lookup"><span data-stu-id="36728-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="36728-121">Og det er meget, at det allerede er lidt for langt.</span><span class="sxs-lookup"><span data-stu-id="36728-121">And this is really already a bit too long.</span></span> <span data-ttu-id="36728-122">Den bedste fremgangsmåde handler om 400 tegn---------------------------------</span><span class="sxs-lookup"><span data-stu-id="36728-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="36728-123">Når dit indhold er klar, skal du trække det til den direkte forgrening.</span><span class="sxs-lookup"><span data-stu-id="36728-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="36728-124">Gå derefter til Alchemy- [partner portalen](https://alchemyportal.azurewebsites.net) , og Indtast filnavnet i feltet URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="36728-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 