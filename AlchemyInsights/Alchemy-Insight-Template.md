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
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800039"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="4ef07-102">Påkrævede Alchemy hovedet H1, H2's virker ikke.</span><span class="sxs-lookup"><span data-stu-id="4ef07-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="4ef07-103">Bedste fremgangsmåder og retningslinjer til oprettelse af Alchemy:</span><span class="sxs-lookup"><span data-stu-id="4ef07-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="4ef07-104">**Kan ikke sammensættes Alchemy indblik i mapper**- det ødelægges URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="4ef07-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="4ef07-105">Vi søger til at løse dette.</span><span class="sxs-lookup"><span data-stu-id="4ef07-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="4ef07-106">Filerne i mappen **AlchemyInsights** skal have små filnavne med bindestreger i mellemrum ex.</span><span class="sxs-lookup"><span data-stu-id="4ef07-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="4ef07-107">***how-til-aktivere-retssag-hold***.</span><span class="sxs-lookup"><span data-stu-id="4ef07-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="4ef07-108">Omfatte regel-ID eller bucket-ID fra [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) i feltet ms.custom.</span><span class="sxs-lookup"><span data-stu-id="4ef07-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="4ef07-109">ex.</span><span class="sxs-lookup"><span data-stu-id="4ef07-109">ex.</span></span> <span data-ttu-id="4ef07-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="4ef07-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="4ef07-111">Brug resten af metadataene i toppen af denne fil som skabelon.</span><span class="sxs-lookup"><span data-stu-id="4ef07-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="4ef07-112">Gå til afsnittet i [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) **kunden indsigt titel:** og brug, der peger som en start til H1 titlen for indsigt.</span><span class="sxs-lookup"><span data-stu-id="4ef07-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="4ef07-113">Alchemy viden skal have en enkelt H1 øverst eller de brydes i produktionen.</span><span class="sxs-lookup"><span data-stu-id="4ef07-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="4ef07-114">H2s gengive ikke, så brug **fed** eller andre konventioner til at angive separate sektioner.</span><span class="sxs-lookup"><span data-stu-id="4ef07-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="4ef07-115">Udfyld derefter brødtekst ved hjælp af udkast til materialet i afsnittet kunden indsigt i siden Alchemy regel</span><span class="sxs-lookup"><span data-stu-id="4ef07-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="4ef07-116">Punktopstillede lister er det fint</span><span class="sxs-lookup"><span data-stu-id="4ef07-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="4ef07-117">Nummererede lister for</span><span class="sxs-lookup"><span data-stu-id="4ef07-117">Numbered lists too</span></span>
    1. <span data-ttu-id="4ef07-118">**Fed** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="4ef07-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="4ef07-119">Links skal altid være en **"links til web" / eksterne** eller **deep-links til elementer i Brugergrænsefladen**, ikke interne hyperlinks.</span><span class="sxs-lookup"><span data-stu-id="4ef07-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="4ef07-120">Billeder understøttes ikke officielt på nuværende tidspunkt, men det er i gang med køreplanen.</span><span class="sxs-lookup"><span data-stu-id="4ef07-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="4ef07-121">Og det er virkelig allerede lidt for langt.</span><span class="sxs-lookup"><span data-stu-id="4ef07-121">And this is really already a bit too long.</span></span> <span data-ttu-id="4ef07-122">Den bedste fremgangsmåde er ca 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="4ef07-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="4ef07-123">Når indholdet er klar, kan du trække det til den levende gren.</span><span class="sxs-lookup"><span data-stu-id="4ef07-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="4ef07-124">Derefter skal du gå til [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) og indtaste filnavnet i feltet URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="4ef07-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 