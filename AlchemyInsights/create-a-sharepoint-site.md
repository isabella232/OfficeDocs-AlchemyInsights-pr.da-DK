---
title: Oprette et SharePoint-websted
ms.author: pebaum
author: todmccoy
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
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770849"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="8fdb1-102">Oprette et SharePoint-websted</span><span class="sxs-lookup"><span data-stu-id="8fdb1-102">Create a SharePoint site</span></span>

<span data-ttu-id="8fdb1-103">Opret eller administrer websteder fra [aktive websteder](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) i SharePoint Administration.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="8fdb1-104">Du kan finde flere oplysninger under [Administrere websteder i den nye SharePoint Administration](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="8fdb1-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="8fdb1-105">Tips:</span><span class="sxs-lookup"><span data-stu-id="8fdb1-105">Tips:</span></span>

- <span data-ttu-id="8fdb1-106">Du **kan ikke** oprette et websted med den samme URL-adresse til et eksisterende websted.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="8fdb1-107">Hvis du har slettet et websted og ønsker at genbruge URL-adressen, er det muligt, at det slettede websted stadig findes under [Slettede websteder](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="8fdb1-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="8fdb1-108">Webstedet skal slettes permanent for at genbruge URL-adressen.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="8fdb1-109">Hvis du vil fjerne et websted helt med Powershell, skal du se eksemplet [fjern-SPSite-cmdlet.](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="8fdb1-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="8fdb1-110">Nogle brugere kan muligvis ikke oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="8fdb1-111">[Se Administrere oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="8fdb1-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="8fdb1-112">Det er muligt, at webstedet vises fast på **Oprettelse** længere end forventet.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="8fdb1-113">Hvis der er gået mere end 24 timer, siden du første gang så dette problem, skal du logge en supportbillet.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8fdb1-114">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8fdb1-115">Giv os mindst 24 timer til at fuldføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="8fdb1-115">Please give us at least 24 hours to complete a solution.</span></span>
