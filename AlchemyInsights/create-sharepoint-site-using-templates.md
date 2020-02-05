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
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770417"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="ec226-102">Oprette SharePoint-websteder ved hjælp af skabeloner</span><span class="sxs-lookup"><span data-stu-id="ec226-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="ec226-103">Muligheden for at gemme et websted som skabelon understøttes ikke med moderne kommunikation eller teamwebsteder.</span><span class="sxs-lookup"><span data-stu-id="ec226-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="ec226-104">Du kan finde flere oplysninger om brug af skabeloner under [Gem, downloade og overføre et SharePoint-websted som en skabelon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="ec226-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="ec226-105">Her er nogle almindelige problemer/løsninger vedrørende lagring af et websted eller en liste som skabelon i Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="ec226-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="ec226-106">**Knappen Gem websteds-/listeskabelon er ikke tilgængelig eller mangler**</span><span class="sxs-lookup"><span data-stu-id="ec226-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="ec226-107">Administratorer skal tillade brugerdefineret script for at aktivere skabelonfunktionerne.</span><span class="sxs-lookup"><span data-stu-id="ec226-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="ec226-108">For detaljerede trin, eksempler og overvejelser se</span><span class="sxs-lookup"><span data-stu-id="ec226-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="ec226-109">Tillad eller forbyt brugerdefineret script</span><span class="sxs-lookup"><span data-stu-id="ec226-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="ec226-110">Kommandoen Gem websted som skabelon understøttes ikke og kan give problemer på websteder, der bruger SharePoint Server Publishing Infrastructure.</span><span class="sxs-lookup"><span data-stu-id="ec226-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="ec226-111">**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**</span><span class="sxs-lookup"><span data-stu-id="ec226-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="ec226-112">Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke.</span><span class="sxs-lookup"><span data-stu-id="ec226-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="ec226-113">Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="ec226-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="ec226-114">Kontroller, om lister eller biblioteker overskrider grænseværdien for grænseværdien for [listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer, da dette kan blokere oprettelsen af en webstedsskabelon.</span><span class="sxs-lookup"><span data-stu-id="ec226-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="ec226-115">Webstedet bruger muligvis for mange ressourcer, og webstedsskabelonen overskrider derfor grænsen på 50 MB.</span><span class="sxs-lookup"><span data-stu-id="ec226-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="ec226-116">Der er problemer med at vise data fra en liste, der bruger en opslagskolonne.</span><span class="sxs-lookup"><span data-stu-id="ec226-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="ec226-117">Du kan finde flere oplysninger under [Listen Skabelongenererede vises ikke data fra den korrekte opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="ec226-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="ec226-118">Du kan finde flere oplysninger om almindelige problemer og løsninger ved at se [Oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="ec226-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



