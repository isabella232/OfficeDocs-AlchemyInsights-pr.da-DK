---
title: Oprette et SharePoint-websted
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786559"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="f2572-102">Oprette et SharePoint-websted</span><span class="sxs-lookup"><span data-stu-id="f2572-102">Create a SharePoint site</span></span>

<span data-ttu-id="f2572-103">Opret eller Administrer websteder fra [aktive websteder](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) i SharePoint-administrations centeret.</span><span class="sxs-lookup"><span data-stu-id="f2572-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="f2572-104">Du kan finde flere oplysninger i [Administrer websteder i den nye SharePoint administration](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f2572-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="f2572-105">Politiktip</span><span class="sxs-lookup"><span data-stu-id="f2572-105">Tips:</span></span>

- <span data-ttu-id="f2572-106">Du **kan ikke** oprette et websted med den samme URL-adresse til et eksisterende websted.</span><span class="sxs-lookup"><span data-stu-id="f2572-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="f2572-107">Hvis du har slettet et websted og ønsker at bruge URL-adressen igen, er det muligt, at det slettede websted stadig findes under [slettede websteder](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="f2572-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="f2572-108">Webstedet skal slettes permanent, for at du kan bruge URL-adressen igen.</span><span class="sxs-lookup"><span data-stu-id="f2572-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="f2572-109">Hvis du vil fjerne et websted helt med PowerShell, skal du se eksemplet [Fjern-SPSite-](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="f2572-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="f2572-110">Nogle brugere vil muligvis ikke kunne oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="f2572-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="f2572-111">[Se Administrer oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f2572-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="f2572-112">Det er muligt, at webstedet ser fast ud, når du **opretter** længere tid end forventet.</span><span class="sxs-lookup"><span data-stu-id="f2572-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="f2572-113">Hvis der er gået mere end 24 timer, siden du først fik dette problem, skal du logge på en support billet.</span><span class="sxs-lookup"><span data-stu-id="f2572-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f2572-114">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="f2572-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f2572-115">Giv os mindst 24 timer for at fuldføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="f2572-115">Please give us at least 24 hours to complete a solution.</span></span>
