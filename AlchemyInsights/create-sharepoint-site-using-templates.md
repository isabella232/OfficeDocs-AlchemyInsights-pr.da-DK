---
title: Oprette et websted i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732211"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="16105-102">Oprette SharePoint-websteder ved hjælp af skabeloner</span><span class="sxs-lookup"><span data-stu-id="16105-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="16105-103">Muligheden for at gemme et websted som en skabelon understøttes ikke med moderne kommunikations-eller team websteder.</span><span class="sxs-lookup"><span data-stu-id="16105-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="16105-104">Du kan finde flere oplysninger om brug af skabeloner i [gemme, hente og overføre et SharePoint-websted som en skabelon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="16105-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="16105-105">Her er nogle almindelige problemer/løsninger i forbindelse med at gemme et websted eller en liste som en skabelon i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="16105-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="16105-106">**Knappen Gem websted/listeskabelon er ikke tilgængelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="16105-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="16105-107">Administratorer skal tillade, at brugerdefineret script aktiverer skabelon funktionerne.</span><span class="sxs-lookup"><span data-stu-id="16105-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="16105-108">Du kan finde detaljerede trin, eksempler og overvejelser i</span><span class="sxs-lookup"><span data-stu-id="16105-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="16105-109">Tillade eller forhindre brugerdefineret script</span><span class="sxs-lookup"><span data-stu-id="16105-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="16105-110">Kommandoen Gem websted som skabelon understøttes ikke og kan medføre problemer på websteder, der bruger SharePoint Server-publicerings infrastrukturen.</span><span class="sxs-lookup"><span data-stu-id="16105-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="16105-111">**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**</span><span class="sxs-lookup"><span data-stu-id="16105-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="16105-112">Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke.</span><span class="sxs-lookup"><span data-stu-id="16105-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="16105-113">Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="16105-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="16105-114">Kontrollér, om lister eller biblioteker overskrider grænseværdien for [listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000-elementer, da dette kan blokere oprettelsen af en webstedsskabelon.</span><span class="sxs-lookup"><span data-stu-id="16105-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="16105-115">Webstedet bruger muligvis for mange ressourcer, og derfor overskrider webstedsskabelonen grænsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="16105-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="16105-116">Der er problemer med at vise data fra en liste, der bruger en opslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="16105-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="16105-117">Hvis du vil have mere at vide, skal du se [listen skabelon oprettet viser ikke data fra den rigtige opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="16105-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="16105-118">Du kan få mere at vide om almindelige problemer og løsninger ved [at se oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="16105-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



