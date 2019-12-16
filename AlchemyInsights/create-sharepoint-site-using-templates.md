---
title: Oprette et websted i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052463"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="3e75b-102">Oprette SharePoint-websteder ved hjælp af skabeloner</span><span class="sxs-lookup"><span data-stu-id="3e75b-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="3e75b-103">SharePoint-webstedsskabeloner er forudbyggede definitioner, der er designet omkring et bestemt forretningsbehov.</span><span class="sxs-lookup"><span data-stu-id="3e75b-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="3e75b-104">Du finder flere oplysninger under [brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="3e75b-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="3e75b-105">Her er nogle almindeligt forekommende problemer/løsninger vedrørende lagring af et websted eller en liste som en skabelon i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3e75b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="3e75b-106">**Knappen Gem websted/listeskabelon er ikke tilgængelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="3e75b-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="3e75b-107">Administratorer skal tillade brugerdefineret script for at aktivere skabelon funktionerne.</span><span class="sxs-lookup"><span data-stu-id="3e75b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="3e75b-108">Detaljerede trin, eksempler og overvejelser findes i</span><span class="sxs-lookup"><span data-stu-id="3e75b-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="3e75b-109">Tillade eller forhindre brugerdefineret script</span><span class="sxs-lookup"><span data-stu-id="3e75b-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="3e75b-110">Kommandoen Gem websted som skabelon understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-Publiceringsinfrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="3e75b-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="3e75b-111">**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**</span><span class="sxs-lookup"><span data-stu-id="3e75b-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="3e75b-112">Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke.</span><span class="sxs-lookup"><span data-stu-id="3e75b-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="3e75b-113">Hvis funktionen ikke er tilgængelig til aktivering i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="3e75b-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="3e75b-114">Kontroller, om lister eller biblioteker overskrider [grænse tærsklen på listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000 elementer, da dette kan blokere oprettelsen af en webstedsskabelon.</span><span class="sxs-lookup"><span data-stu-id="3e75b-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="3e75b-115">Webstedet bruger muligvis for mange ressourcer, og webstedsskabelonen overskrider derfor grænsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="3e75b-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="3e75b-116">Der er problemer med at vise data fra en liste, der bruger en opslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="3e75b-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="3e75b-117">Du finder flere oplysninger under [skabelon genereret liste viser ikke data fra den korrekte opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="3e75b-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="3e75b-118">Du kan finde mere detaljerede oplysninger om almindeligt forekommende problemer og løsninger ved at kontrollere [Opret og brug webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="3e75b-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



