---
title: For overførsel af offentlige mapper til batch med CompletedWithErrors-status
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744107"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>For overførsel af offentlige mapper til batch med CompletedWithErrors-status

Benyt følgende fremgangsmåde for at fuldføre batchen ved at springe over de store/dårlige elementer: 
1. Godkend de elementer, der blev sprunget over, ved overførselsbatch:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Brug følgende kommando til at godkende de elementer, der blev sprunget over ved overførsels anmodninger, som er "synkroniserede", men ikke fuldført:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Overførsels batchen og anmodningerne skal genoptages og afsluttes om et par minutter.

