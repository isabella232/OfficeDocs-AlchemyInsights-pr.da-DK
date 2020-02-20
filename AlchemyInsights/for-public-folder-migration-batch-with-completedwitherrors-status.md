---
title: For batch til overførsel af offentlige mapper med statussen FuldførtEfejl
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
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158595"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="f78ec-102">For batch til overførsel af offentlige mapper med statussen FuldførtEfejl</span><span class="sxs-lookup"><span data-stu-id="f78ec-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="f78ec-103">Brug følgende trin til at fuldføre batchen og springe de store/beskadigede elementer over:</span><span class="sxs-lookup"><span data-stu-id="f78ec-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="f78ec-104">Godkend de oversprungne varer på overførselsbatch:</span><span class="sxs-lookup"><span data-stu-id="f78ec-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="f78ec-105">Brug følgende kommando til at godkende de elementer, der er sprunget over på overførselsanmodninger, der er "Synkroniseret", men ikke fuldført:</span><span class="sxs-lookup"><span data-stu-id="f78ec-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="f78ec-106">Overførselsbatchen og anmodningerne skal genoptages og afsluttes om nogle få minutter.</span><span class="sxs-lookup"><span data-stu-id="f78ec-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

