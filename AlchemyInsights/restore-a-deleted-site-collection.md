---
title: Gendanne et slettet websted
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692037"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="fab2c-102">Gendanne et slettet websted</span><span class="sxs-lookup"><span data-stu-id="fab2c-102">Restore a deleted site</span></span>

<span data-ttu-id="fab2c-103">Når en administrator sletter et SharePoint-websted, er det placeret i papirkurven for gruppen af websteder, hvor det opbevares i 93 dage, før det slettes permanent.</span><span class="sxs-lookup"><span data-stu-id="fab2c-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="fab2c-104">Sådan gendannes webstedet:</span><span class="sxs-lookup"><span data-stu-id="fab2c-104">To restore the site:</span></span>
  
1. <span data-ttu-id="fab2c-105">I den nye SharePoint administration skal du klikke på **Papirkurv** på båndet.</span><span class="sxs-lookup"><span data-stu-id="fab2c-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="fab2c-106">Markér afkrydsningsfeltet ud for den gruppe af websteder, du vil gendanne.</span><span class="sxs-lookup"><span data-stu-id="fab2c-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="fab2c-107">Klik på **Gendan slettede elementer**.</span><span class="sxs-lookup"><span data-stu-id="fab2c-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="fab2c-108">Hvis du vil gendanne et slettet kommunikationswebsted, kan du bruge den nye SharePoint administration.</span><span class="sxs-lookup"><span data-stu-id="fab2c-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="fab2c-109">Ellers skal du bruge Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fab2c-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="fab2c-110">Hvis du vil gendanne et websted, der tilhører en Microsoft 365-gruppe, skal du gendanne gruppen i Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="fab2c-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="fab2c-111">Grupper kan gendannes i 30 dage, efter at de er blevet slettet.</span><span class="sxs-lookup"><span data-stu-id="fab2c-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

