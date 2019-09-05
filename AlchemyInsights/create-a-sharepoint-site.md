---
title: Oprette et SharePoint-websted
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738191"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="f0937-102">Oprette et SharePoint-websted</span><span class="sxs-lookup"><span data-stu-id="f0937-102">Create a SharePoint site</span></span>

<span data-ttu-id="f0937-103">Du kan se følgende oplysninger om oprettelse af SharePoint-websteder:</span><span class="sxs-lookup"><span data-stu-id="f0937-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="f0937-104">[Administrer websteder i det nye SharePoint-Administrationscenter](https://docs.microsoft.com/sharepoint/manage-site-creation): få mere at vide om indstillinger for oprettelse af websteder, herunder hvordan du opretter et klassisk websted eller et teams-websted, der ikke indeholder en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="f0937-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="f0937-105">[Opret et teamwebsted i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): få mere at vide om, hvordan du opretter et teamwebsted.</span><span class="sxs-lookup"><span data-stu-id="f0937-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="f0937-106">[Opret et kommunikationswebsted i SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): få mere at vide om, hvordan du opretter et kommunikationswebsted.</span><span class="sxs-lookup"><span data-stu-id="f0937-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="f0937-107">[Administrer websteder i det nye SharePoint-Administrationscenter](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): få mere at vide om, hvordan du opretter et klassisk websted eller et teamwebsted, der ikke indeholder en Office 365-gruppe.</span><span class="sxs-lookup"><span data-stu-id="f0937-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="f0937-108">[! Tips</span><span class="sxs-lookup"><span data-stu-id="f0937-108">[!Tips]</span></span>
> - <span data-ttu-id="f0937-109">Du kan ikke oprette et websted med den samme URL-adresse til et eksisterende websted.</span><span class="sxs-lookup"><span data-stu-id="f0937-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="f0937-110">Hvis du har slettet et websted og ønsker at genbruge WEBADRESSEN, er det muligt, at det slettede websted stadig findes under **slettede websteder**.</span><span class="sxs-lookup"><span data-stu-id="f0937-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="f0937-111">Hvis du vil administrere slettede websteder, skal [du slette et websted](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="f0937-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="f0937-112">Hvis du helt vil fjerne et websted med PowerShell, skal du se eksemplet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="f0937-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="f0937-113">Nogle brugere vil muligvis ikke kunne oprette et websted.</span><span class="sxs-lookup"><span data-stu-id="f0937-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="f0937-114">Se [Administrer oprettelse af websteder i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="f0937-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="f0937-115">Det er muligt, at webstedet vises fast på **at oprette** længere end forventet.</span><span class="sxs-lookup"><span data-stu-id="f0937-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="f0937-116">Hvis der er gået mere end 24 timer, siden du så dette problem, skal du logge en support billet.</span><span class="sxs-lookup"><span data-stu-id="f0937-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f0937-117">I mange tilfælde arbejder vi allerede på en løsning.</span><span class="sxs-lookup"><span data-stu-id="f0937-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f0937-118">Giv os mindst 24 timer til at gennemføre en løsning.</span><span class="sxs-lookup"><span data-stu-id="f0937-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="f0937-119">Hvis du har brug for at oprette et nyt teamwebsted, der ikke indeholder en Office 365-gruppe,</span><span class="sxs-lookup"><span data-stu-id="f0937-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


