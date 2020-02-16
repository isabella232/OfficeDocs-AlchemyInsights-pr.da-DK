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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043577"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>For batch til overførsel af offentlige mapper med statussen FuldførtEfejl

Brug følgende trin til at fuldføre batchen og springe de store/beskadigede elementer over: 
1. Godkend de oversprungne varer på overførselsbatch:

    Batchnavn set-migrationBatch \<> -Godkend sprunget poster 
2. Brug følgende kommando til at godkende de elementer, der er sprunget over på overførselsanmodninger, der er "Synkroniseret", men ikke fuldført:

    $pf=Get-PublicFolderMailboxMigrationRequest | Hent-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForHver ($i i $pf) {hvis ($i.LargeItemsFundet -gt 0 -eller $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}
3. Overførselsbatchen og anmodningerne skal genoptages og afsluttes om nogle få minutter.

