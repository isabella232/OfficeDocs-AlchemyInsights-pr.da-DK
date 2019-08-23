---
title: Gemme webstedet eller listen som en skabelon
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551625"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="3c494-102">Gemme webstedet eller listen som en skabelon</span><span class="sxs-lookup"><span data-stu-id="3c494-102">Save site or list as a template</span></span>

<span data-ttu-id="3c494-103">SharePoint-websted-skabeloner er færdige definitioner, der er designet omkring et bestemt behov i virksomheden.</span><span class="sxs-lookup"><span data-stu-id="3c494-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="3c494-104">Yderligere oplysninger finder du under [Brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="3c494-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="3c494-105">Her er nogle almindelige problemer/løsninger med hensyn til lagring af et websted eller en liste som skabelon i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3c494-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="3c494-106">**Gem websted/denne liste skabelon knap er ikke tilgængelig eller mangler**.</span><span class="sxs-lookup"><span data-stu-id="3c494-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="3c494-107">Administratorer skal tillade brugerdefineret Script til at aktivere Skabelonfunktioner på.</span><span class="sxs-lookup"><span data-stu-id="3c494-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="3c494-108">Se flere detaljerede oplysninger, eksempler og overvejelser i forbindelse med [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="3c494-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="3c494-109">Gem webstedet som skabelon-kommando understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-udgivelse-infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="3c494-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="3c494-110">**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**</span><span class="sxs-lookup"><span data-stu-id="3c494-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="3c494-111">Skabelonen mangler en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og kan ikke aktiveres.</span><span class="sxs-lookup"><span data-stu-id="3c494-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="3c494-112">Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen for at oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="3c494-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="3c494-113">Kontrollere Hvis lister og biblioteker, overstiger den [Grænse for listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) af 5000 varer som dette kan blokere for oprettelse af en webstedsskabelon.</span><span class="sxs-lookup"><span data-stu-id="3c494-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="3c494-114">Webstedet bruger måske for mange ressourcer, og derfor webstedsskabelonen overskrider grænsen på 50 MB (Megabyte).</span><span class="sxs-lookup"><span data-stu-id="3c494-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="3c494-115">Der er problemer med at vise data fra en liste, der bruger en opslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="3c494-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="3c494-116">Yderligere oplysninger finder du i [skabelon-genereret liste ikke viser data fra den korrekte opslagsliste i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="3c494-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="3c494-117">For mere detaljerede oplysninger om almindelige problemer og løsninger, skal du reference, [oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="3c494-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

