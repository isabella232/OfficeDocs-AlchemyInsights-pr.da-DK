---
title: Oprette et websted i SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753701"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="38cc5-102">Oprette SharePoint-websteder ved hjælp af skabeloner</span><span class="sxs-lookup"><span data-stu-id="38cc5-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="38cc5-103">SharePoint-websted-skabeloner er færdige definitioner, der er designet omkring et bestemt behov i virksomheden.</span><span class="sxs-lookup"><span data-stu-id="38cc5-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="38cc5-104">Yderligere oplysninger finder du under [Brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="38cc5-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="38cc5-105">Her er nogle almindelige problemer/løsninger med hensyn til lagring af et websted eller en liste som skabelon i Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="38cc5-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="38cc5-106">**Knappen Gem websted/denne liste skabelon er ikke tilgængelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="38cc5-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="38cc5-107">Administratorer skal tillade brugerdefineret Script til at aktivere Skabelonfunktioner på.</span><span class="sxs-lookup"><span data-stu-id="38cc5-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="38cc5-108">Se for detaljerede trin, eksempler og overvejelser</span><span class="sxs-lookup"><span data-stu-id="38cc5-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="38cc5-109">Tillade eller forhindre brugerdefineret script</span><span class="sxs-lookup"><span data-stu-id="38cc5-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="38cc5-110">Gem webstedet som skabelon-kommando understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-udgivelse-infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="38cc5-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="38cc5-111">Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt.</span><span class="sxs-lookup"><span data-stu-id="38cc5-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="38cc5-112">Skabelonen mangler en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og kan ikke aktiveres.</span><span class="sxs-lookup"><span data-stu-id="38cc5-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="38cc5-113">Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen for at oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="38cc5-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="38cc5-114">Kontrollere Hvis lister og biblioteker, overstiger den [Grænse for listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) af 5000 varer som dette kan blokere for oprettelse af en webstedsskabelon.</span><span class="sxs-lookup"><span data-stu-id="38cc5-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="38cc5-115">Webstedet bruger måske for mange ressourcer, og derfor webstedsskabelonen overskrider grænsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="38cc5-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="38cc5-116">Der er problemer med at vise data fra en liste, der bruger en opslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="38cc5-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="38cc5-117">Yderligere oplysninger finder du i [skabelon-genereret liste ikke viser data fra den korrekte opslagsliste i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="38cc5-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="38cc5-118">Mere detaljerede oplysninger om almindelige problemer og løsninger, skal du kontrollere [oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="38cc5-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



