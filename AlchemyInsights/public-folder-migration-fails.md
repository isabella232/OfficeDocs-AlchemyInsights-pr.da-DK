---
title: Overførsel af offentlige mapper mislykkes ved 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803493"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="99a70-102">Overførsel af offentlige mapper mislykkes ved 95%</span><span class="sxs-lookup"><span data-stu-id="99a70-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="99a70-103">Du har muligvis indledt fuldførelsen af en overførselsbatch, og status for overførsels batchen fortsætter med at blive **synkroniseret** i meget lang tid.</span><span class="sxs-lookup"><span data-stu-id="99a70-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="99a70-104">Dette er den forventede funktionsmåde.</span><span class="sxs-lookup"><span data-stu-id="99a70-104">This is expected behavior.</span></span>

<span data-ttu-id="99a70-105">Det er almindeligt for en overførsels batchs status at forblive **synkroniseret** for et par timer, før den skifter til **fuldførelse**.</span><span class="sxs-lookup"><span data-stu-id="99a70-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="99a70-106">For overførsler, der omfatter et stort antal destinations postkasser, er det normalt at se status forbliver i synkroniseret tilstand i mere end 24 timer, forudsat at ingen af de underliggende anmodninger om overførsel af offentlige mapper mislykkedes eller var i karantæne.</span><span class="sxs-lookup"><span data-stu-id="99a70-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="99a70-107">Tillad 24-48 timer for overførsels batchen for at fuldføre opgaverne.</span><span class="sxs-lookup"><span data-stu-id="99a70-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="99a70-108">For overførsler af offentlige mapper, der mislykkedes på 95%, med fejl FailedToMailEnablePublicFoldersException:</span><span class="sxs-lookup"><span data-stu-id="99a70-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="99a70-109">Download og Kør [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) -scriptet på din Exchange-Server i det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="99a70-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="99a70-110">Udføre de rette handlinger, der foreslås af scriptet.</span><span class="sxs-lookup"><span data-stu-id="99a70-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="99a70-111">Kør Sync-MailPublicFolders (for Exchange 2010) eller sync-ModernMailPublicFolders (for Exchange 2013 og nyere).</span><span class="sxs-lookup"><span data-stu-id="99a70-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="99a70-112">Genoptag overførsel af offentlige mapper.</span><span class="sxs-lookup"><span data-stu-id="99a70-112">Resume public folder migration.</span></span>
