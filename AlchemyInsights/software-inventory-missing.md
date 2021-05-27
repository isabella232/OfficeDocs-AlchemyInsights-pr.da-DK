---
title: Softwarelager mangler eller er unøjagtigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676142"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="f9e0e-102">Softwarelager mangler eller er unøjagtigt</span><span class="sxs-lookup"><span data-stu-id="f9e0e-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="f9e0e-103">Softwarelageret på Håndtering af trusler og sikkerhedsrisici (TVM) er en liste over kendt software i din organisation med officielle Common Platform Enumerations (CPE).</span><span class="sxs-lookup"><span data-stu-id="f9e0e-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="f9e0e-104">Softwareprodukter uden en officiel CPE har ikke offentliggjort sårbarheder.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="f9e0e-105">Lageret indeholder også oplysninger som f.eks. navnet på leverandøren, antallet af personer, trusler og antallet af enheder, der vises.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="f9e0e-106">Softwareændringer på enheder afspejles typisk i sikkerhedsportaler inden for to timer.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="f9e0e-107">Men det kan nogle gange tage længere tid.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="f9e0e-108">Det er i øjeblikket ikke muligt at gennemtvinge en synkronisering. dette er en løbende løbende vurdering.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="f9e0e-109">Hvis du har foretaget en softwareændring, og ændringen ikke afspejles nøjagtigt i TVM efter 5 timer, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="f9e0e-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="f9e0e-110">Kontrollér afsnittet om software beviser for at forstå, hvordan softwaren blev registreret.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="f9e0e-111">Sørg for, at softwaren understøttes.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-111">Make sure that the software is supported.</span></span> <span data-ttu-id="f9e0e-112">Software kan kun ses på enhedsniveau, selvom det i øjeblikket ikke understøttes af Håndtering af trusler og sikkerhedsrisici.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="f9e0e-113">Men kun begrænsede data er tilgængelige.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="f9e0e-114">Du kan finde en vejledning til, hvordan du rapporterer unøjagtigheden fra portalen, [under Rapport om unøjagtighed.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="f9e0e-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="f9e0e-115">**Bemærk!** Rapportering af en unøjagtighed fra MDE-portalen er en envejskanal til tekniker.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="f9e0e-116">Hvis problemet haster, skal du åbne en supportanmodning.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="f9e0e-117">Du kan finde flere oplysninger [i Softwarelager – Håndtering af trusler og sikkerhedsrisici](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="f9e0e-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>