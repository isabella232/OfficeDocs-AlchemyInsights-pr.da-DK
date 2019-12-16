---
title: Gem websted eller liste som en skabelon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048718"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="7cd94-102">Gem websted eller liste som en skabelon</span><span class="sxs-lookup"><span data-stu-id="7cd94-102">Save site or list as a template</span></span>

<span data-ttu-id="7cd94-103">SharePoint-webstedsskabeloner er forudbyggede definitioner, der er designet omkring et bestemt forretningsbehov.</span><span class="sxs-lookup"><span data-stu-id="7cd94-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="7cd94-104">Du finder flere oplysninger under [brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="7cd94-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="7cd94-105">Her er nogle almindeligt forekommende problemer/løsninger vedrørende lagring af et websted eller en liste som en skabelon i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="7cd94-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="7cd94-106">**Knappen Gem websted/listeskabelon er ikke tilgængelig eller mangler**.</span><span class="sxs-lookup"><span data-stu-id="7cd94-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="7cd94-107">Administratorer skal tillade brugerdefineret script for at aktivere skabelon funktionerne.</span><span class="sxs-lookup"><span data-stu-id="7cd94-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="7cd94-108">Du kan finde detaljerede trin, eksempler og overvejelser under [tillade eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="7cd94-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="7cd94-109">Kommandoen Gem websted som skabelon understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-Publiceringsinfrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="7cd94-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="7cd94-110">**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**</span><span class="sxs-lookup"><span data-stu-id="7cd94-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="7cd94-111">Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke.</span><span class="sxs-lookup"><span data-stu-id="7cd94-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="7cd94-112">Hvis funktionen ikke er tilgængelig til aktivering i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="7cd94-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="7cd94-113">Kontroller, om lister eller biblioteker overskrider [grænse tærsklen på listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000 elementer, da dette kan blokere oprettelsen af en webstedsskabelon.</span><span class="sxs-lookup"><span data-stu-id="7cd94-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="7cd94-114">Webstedet bruger muligvis for mange ressourcer, og webstedsskabelonen overskrider derfor grænsen på 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="7cd94-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="7cd94-115">Der er problemer med at vise data fra en liste, der bruger en opslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="7cd94-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="7cd94-116">Du finder flere oplysninger under [skabelon genereret liste viser ikke data fra den korrekte opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="7cd94-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="7cd94-117">For mere detaljerede oplysninger om almindeligt forekommende problemer og løsninger henvises til, [Opret og brug webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="7cd94-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

