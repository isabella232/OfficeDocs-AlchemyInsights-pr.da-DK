---
title: Repliker sæt
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713750"
---
# <a name="replica-set"></a><span data-ttu-id="e6e7d-102">Repliker sæt</span><span class="sxs-lookup"><span data-stu-id="e6e7d-102">Replica set</span></span>

<span data-ttu-id="e6e7d-103">AADDS kaldes også for det administrerede domæne.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="e6e7d-104">Det er faktisk to domænecontrollere, der køres og vedligeholdes af backend.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="e6e7d-105">De to DCs omfatter én hoved-DC og én replikerings-DC.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="e6e7d-106">Sikkerhedskopier i AADDS (administreret domæne) er en automatiseret proces, der administreres af Azure-platformen.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="e6e7d-107">I tilfælde af et problem med dit administrerede domæne kan Azure-support hjælpe dig med at gendanne fra sikkerhedskopien.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="e6e7d-108">Du opretter hvert replikeringssæt i et virtuelt netværk.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="e6e7d-109">Hvert virtuelt netværk skal peeres til alle andre virtuelle netværk, der hoster et administreret domænes replikeringssæt.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="e6e7d-110">Denne konfiguration opretter en netværktopologi til net, der understøtter katalogreplikering.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="e6e7d-111">Et virtuelt netværk kan understøtte flere replikeringssæt, forudsat at hvert replikeringssæt er i et andet virtuelt undernet.</span><span class="sxs-lookup"><span data-stu-id="e6e7d-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="e6e7d-112">Du kan finde flere oplysninger om replikeringssæt i [Concepts Replica-sæt.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="e6e7d-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
