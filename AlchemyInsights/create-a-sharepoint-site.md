---
title: Oprette et SharePoint-websted
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802960"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="26b8d-102">Oprette et SharePoint-websted</span><span class="sxs-lookup"><span data-stu-id="26b8d-102">Create a SharePoint site</span></span>

<span data-ttu-id="26b8d-103">Du kan se følgende oplysninger om oprettelse af SharePoint-websted:</span><span class="sxs-lookup"><span data-stu-id="26b8d-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="26b8d-104">[Administrer websteder i det nye SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Få mere at vide om webstedet oprettelse af muligheder, herunder hvordan du opretter en klassisk websted eller et websted for team, der ikke indeholder en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="26b8d-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="26b8d-105">[Opret et websted for team i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Lær, hvordan du opretter et teamwebsted.</span><span class="sxs-lookup"><span data-stu-id="26b8d-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="26b8d-106">[Opret en kommunikationswebsted i SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Lær, hvordan du opretter et websted til kommunikation.</span><span class="sxs-lookup"><span data-stu-id="26b8d-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="26b8d-107">[Administrer websteder i det nye SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Lær, hvordan du opretter et klassisk websted eller et websted for team, der ikke indeholder en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="26b8d-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Tip]
> - <span data-ttu-id="26b8d-109">Du kan ikke oprette et websted med samme URL-adresse på et eksisterende websted.</span><span class="sxs-lookup"><span data-stu-id="26b8d-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="26b8d-110">Hvis du har slettet et websted og der ønsker at genbruge URL-adressen, kan webstedet slettede stadig findes under **websteder slettes**.</span><span class="sxs-lookup"><span data-stu-id="26b8d-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="26b8d-111">Slettet steder se, [slette et websted](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)til at administrere.</span><span class="sxs-lookup"><span data-stu-id="26b8d-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="26b8d-112">Hvis du vil fjerne et websted med Powershell fuldstændigt, se eksemplet med [Fjern-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) -cmdlet.</span><span class="sxs-lookup"><span data-stu-id="26b8d-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="26b8d-113">Nogle brugere muligvis ikke at oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="26b8d-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="26b8d-114">Se [Administrer websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="26b8d-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="26b8d-115">Det er muligt, at webstedet vises fastlåste ved **oprettelse af** længere tid end forventet.</span><span class="sxs-lookup"><span data-stu-id="26b8d-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="26b8d-116">Hvis der er gået mere end 24 timer, da du så først problemet, skal du logge en støtte billet.</span><span class="sxs-lookup"><span data-stu-id="26b8d-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="26b8d-117">I mange tilfælde kan arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="26b8d-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="26b8d-118">Giv os, mindst 24 timer at gennemføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="26b8d-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="26b8d-119">Hvis du vil oprette et nyt websted for team, der ikke indeholder en Office 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="26b8d-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


