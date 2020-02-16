---
title: Gendanne en slettet offentlig mappe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063622"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="27daa-102">Gendanne en slettet offentlig mappe</span><span class="sxs-lookup"><span data-stu-id="27daa-102">Restore a deleted public folder</span></span>

<span data-ttu-id="27daa-103">**Sådan gendannes slettede elementer fra en offentlig mappe:**</span><span class="sxs-lookup"><span data-stu-id="27daa-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="27daa-104">Se [Du kan ikke gendanne slettede elementer fra en offentlig mappe, der ikke er e-mail, i Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="27daa-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="27daa-105">**Sådan gendannes en slettet offentlig mappe (af enhver type):**</span><span class="sxs-lookup"><span data-stu-id="27daa-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="27daa-106">Brug følgende EXO PowerShell-kommando:</span><span class="sxs-lookup"><span data-stu-id="27daa-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="27daa-107">Syntaks:</span><span class="sxs-lookup"><span data-stu-id="27daa-107">Syntax:</span></span>

    ><span data-ttu-id="27daa-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Navn -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Stisti, hvor mappen gendannes></span><span class="sxs-lookup"><span data-stu-id="27daa-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="27daa-109">Eksempel: Følgende kommando gendanner Undermappe1 og placerer den under \Parent1:</span><span class="sxs-lookup"><span data-stu-id="27daa-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="27daa-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Navn -eq "Undermappe1"}; Set-PublicFolder $pf.identity -Sti \Parent1</span><span class="sxs-lookup"><span data-stu-id="27daa-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="27daa-111">Se [Gendanne en slettet offentlig mappe](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="27daa-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
