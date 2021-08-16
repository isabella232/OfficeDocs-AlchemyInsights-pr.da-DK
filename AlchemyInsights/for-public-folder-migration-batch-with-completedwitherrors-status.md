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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068158"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Ved overførselsbatch til offentlig mappe med statussen CompletedWithErrors

Brug følgende trin til at fuldføre batchen og springe de store/dårlige elementer over: 
1. Godkend de ignorerede elementer i overførselsbatchen:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Brug følgende kommando til at godkende de ignorerede elementer ved overførselsanmodninger, der er "synkroniseret", men ikke fuldført:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Overførselsbatchen og anmodningerne bør genoptages og fuldføres om et par minutter.

