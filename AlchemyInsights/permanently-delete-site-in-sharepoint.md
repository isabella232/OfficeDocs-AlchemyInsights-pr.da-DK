---
title: Slet et websted permanent i SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955130"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="5920a-102">Slet et websted permanent i SharePoint</span><span class="sxs-lookup"><span data-stu-id="5920a-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="5920a-103">Hvis du vil genbruge en webadresse fra et slettet websted (for at genskabe et websted) eller permanent slette et websted, fordi det ikke længere er i brug,kan du bruge **Slet permanent** fra det nye SharePoint Administration.</span><span class="sxs-lookup"><span data-stu-id="5920a-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="5920a-104">Gå til [siden Slettede websteder i det nye SharePoint Administration](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true), og log på med en konto, der har administratortilladelser for din organisation.</span><span class="sxs-lookup"><span data-stu-id="5920a-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="5920a-105">Markér et websted i venstre kolonne.</span><span class="sxs-lookup"><span data-stu-id="5920a-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="5920a-106">Klik på **Slet permanent**.</span><span class="sxs-lookup"><span data-stu-id="5920a-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="5920a-107">**Bemærk**: Gruppe-forbundne websteder kan ikke slettes permanent fra det nye SharePoint Administration.</span><span class="sxs-lookup"><span data-stu-id="5920a-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="5920a-108">Du skal bruge [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) i stedet.</span><span class="sxs-lookup"><span data-stu-id="5920a-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="5920a-109">Hvis du vil have flere oplysninger, skal du se [Slet et websted permanent](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="5920a-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
