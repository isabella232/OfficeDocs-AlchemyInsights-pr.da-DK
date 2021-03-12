---
title: Stop automatisk flytning af meddelelser til arkivet
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744671"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="d7d3e-102">Stop automatisk flytning af meddelelser til arkivet</span><span class="sxs-lookup"><span data-stu-id="d7d3e-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="d7d3e-103">Hvis du bruger en opbevaringspolitik, kan du ændre opbevaringsalderen i den pågældende politik, så meddelelser ikke arkiveres automatisk.</span><span class="sxs-lookup"><span data-stu-id="d7d3e-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="d7d3e-104">Sådan gør du:</span><span class="sxs-lookup"><span data-stu-id="d7d3e-104">Here's how:</span></span>

1. <span data-ttu-id="d7d3e-105">Vælg [opbevaringsmærker for overholdelsesstyring](https://go.microsoft.com/fwlink/?linkid=2059104)i Exchange   >  **Administration.**</span><span class="sxs-lookup"><span data-stu-id="d7d3e-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="d7d3e-106">Find dit Flyt til Arkiv-opbevaringsmærke.</span><span class="sxs-lookup"><span data-stu-id="d7d3e-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="d7d3e-107">I opbevaringsmærket skal du ændre opbevaringsperioden  (arkiveringsperioden) til Aldrig for at forhindre elementer i at blive arkiveret automatisk af en opbevaringspolitik.</span><span class="sxs-lookup"><span data-stu-id="d7d3e-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="d7d3e-108">Dette ændrer indstillingen for arkiv for alle postkasser, hvor dette opbevaringsmærke er anvendt på dem.</span><span class="sxs-lookup"><span data-stu-id="d7d3e-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
