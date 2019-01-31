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
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662924"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="31d3b-102">Virker ikke kræves kunde modstående H1, H2</span><span class="sxs-lookup"><span data-stu-id="31d3b-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="31d3b-103">Eksempel på tekst blokere - Følg disse instruktioner:</span><span class="sxs-lookup"><span data-stu-id="31d3b-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="31d3b-104">Filerne i mappen **AlchemyInsights** skal have regel-ID og navn på regel fra [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.</span><span class="sxs-lookup"><span data-stu-id="31d3b-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="31d3b-p101">f.eks. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="31d3b-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="31d3b-p102">Brug metadataene i toppen af denne fil som skabelon. Intet andet er påkrævet.</span><span class="sxs-lookup"><span data-stu-id="31d3b-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="31d3b-109">Gå til afsnittet i [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) **kunden indsigt titel:** og brug, der peger som en start til H1 titlen for indsigt.</span><span class="sxs-lookup"><span data-stu-id="31d3b-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="31d3b-p103">Alchemy viden skal have en enkelt H1 øverst eller de brydes i produktionen. H2s gengive ikke, så brug **fed** eller andre konventioner til at angive separate sektioner.</span><span class="sxs-lookup"><span data-stu-id="31d3b-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="31d3b-112">Udfyld derefter brødtekst ved hjælp af udkast til materialet i afsnittet kunden indsigt i siden Alchemy regel</span><span class="sxs-lookup"><span data-stu-id="31d3b-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="31d3b-113">Punktopstillede lister er det fint</span><span class="sxs-lookup"><span data-stu-id="31d3b-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="31d3b-114">Nummererede lister for</span><span class="sxs-lookup"><span data-stu-id="31d3b-114">Numbered lists too</span></span>
    1. <span data-ttu-id="31d3b-115">**Fed** og *kursiv* er a-ok</span><span class="sxs-lookup"><span data-stu-id="31d3b-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="31d3b-116">Links skal altid være en **"links til web" / eksterne** eller **deep-links til elementer i Brugergrænsefladen**, ikke interne hyperlinks.</span><span class="sxs-lookup"><span data-stu-id="31d3b-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="31d3b-p104">Og det er virkelig allerede lidt for langt. Den bedste fremgangsmåde er ca 400 tegn---</span><span class="sxs-lookup"><span data-stu-id="31d3b-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="31d3b-p105">Når indholdet er klar, kan du trække det til den levende gren. Derefter skal du gå til [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) og indtaste filnavnet i feltet URL-adresse. Kontroller, at indsigt, revideres og offentliggøres, siger "Ja", og klik derefter på Opdater regel. (Det ser pænere i den nye version af portalen - udgiver snart.)</span><span class="sxs-lookup"><span data-stu-id="31d3b-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL-feltet](media/for-content-team.PNG)

