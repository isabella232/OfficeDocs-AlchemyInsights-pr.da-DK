---
title: 'samme som filnavn er bedst [regel #-beskrivelse]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697124"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="85191-102">Påkrævede Alchemy hovedet H1, H2's virker ikke.</span><span class="sxs-lookup"><span data-stu-id="85191-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="85191-103">Bedste fremgangsmåder og retningslinjer til oprettelse af Alchemy:</span><span class="sxs-lookup"><span data-stu-id="85191-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="85191-p101">**Kan ikke sammensættes Alchemy indblik i mapper**- det ødelægges URL-strukturen. Vi søger til at løse dette.</span><span class="sxs-lookup"><span data-stu-id="85191-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="85191-106">Filerne i mappen **AlchemyInsights** skal have regel-ID og navn på regel fra [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.</span><span class="sxs-lookup"><span data-stu-id="85191-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="85191-p102">f.eks. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="85191-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="85191-p103">Brug metadataene i toppen af denne fil som skabelon. Intet andet er påkrævet.</span><span class="sxs-lookup"><span data-stu-id="85191-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="85191-111">Gå til afsnittet i [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) **kunden indsigt titel:** og brug, der peger som en start til H1 titlen for indsigt.</span><span class="sxs-lookup"><span data-stu-id="85191-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="85191-p104">Alchemy viden skal have en enkelt H1 øverst eller de brydes i produktionen. H2s gengive ikke, så brug **fed** eller andre konventioner til at angive separate sektioner.</span><span class="sxs-lookup"><span data-stu-id="85191-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="85191-114">Udfyld derefter brødtekst ved hjælp af udkast til materialet i afsnittet kunden indsigt i siden Alchemy regel</span><span class="sxs-lookup"><span data-stu-id="85191-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="85191-115">Punktopstillede lister er det fint</span><span class="sxs-lookup"><span data-stu-id="85191-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="85191-116">Nummererede lister for</span><span class="sxs-lookup"><span data-stu-id="85191-116">Numbered lists too</span></span>
    1. <span data-ttu-id="85191-117">**Fed** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="85191-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="85191-118">Links skal altid være en **"links til web" / eksterne** eller **deep-links til elementer i Brugergrænsefladen**, ikke interne hyperlinks.</span><span class="sxs-lookup"><span data-stu-id="85191-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="85191-p105">Og det er virkelig allerede lidt for langt. Den bedste fremgangsmåde er ca 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="85191-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="85191-p106">Når indholdet er klar, kan du trække det til den levende gren. Derefter skal du gå til [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) og indtaste filnavnet i feltet URL-adresse. Kontroller, at indsigt, revideres og offentliggøres, siger "Ja", og klik derefter på Opdater regel. **(Det ser pænere i den nye version af portalen - udgiver snart.)** 
 ![URL-felt](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="85191-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

