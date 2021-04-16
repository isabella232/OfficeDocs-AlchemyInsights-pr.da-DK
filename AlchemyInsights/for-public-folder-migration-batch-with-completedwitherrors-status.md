---
title: Ved overførselsbatch til offentlig mappe med statussen CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812458"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Ved overførselsbatch til offentlig mappe med statussen CompletedWithErrors

Brug følgende trin til at fuldføre batchen og springe de store/dårlige elementer over: 
1. Godkend de ignorerede elementer i overførselsbatchen:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Brug følgende kommando til at godkende de ignorerede elementer ved overførselsanmodninger, der er "synkroniseret", men ikke fuldført:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Overførselsbatchen og anmodningerne bør genoptages og fuldføres om et par minutter.

