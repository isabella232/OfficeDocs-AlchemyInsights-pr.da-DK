---
title: Overvågning af betinget adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708668"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="5a0fb-102">Overvågning af betinget adgang til Exchange</span><span class="sxs-lookup"><span data-stu-id="5a0fb-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="5a0fb-103">Brugere, der er målrettet betinget adgang, modtager en mail, hvis de ikke opfylder din organisations adgangskrav.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="5a0fb-104">For at løse dette anbefaler vi en eller flere af følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="5a0fb-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="5a0fb-105">Hvis enheden antages at være tilmeldt, skal du opfordre brugeren til at gå til appen Firmaportal og kontrollere, at den vises i firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="5a0fb-106">Hvis det ikke er muligt, skal brugeren tilmelde enheden.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="5a0fb-107">I Azure-portalen skal du gå til Intune > overholdelse af enhed.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="5a0fb-108">Klik på Enhedsoverholdelse under Skærm.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="5a0fb-109">Få vist overholdelsesrapporten for enheden for at bekræfte, at brugerens enhed er markeret som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="5a0fb-110">I Azure-portalen skal du gå til Intune > overholdelse af enhed.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="5a0fb-111">Klik på Politikker under Administrer.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-111">Under Manage, click Policies.</span></span> <span data-ttu-id="5a0fb-112">Kontrollér, at der er tildelt en profil til brugerens enhed på listen over politikker for overholdelse af regler og standarder.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="5a0fb-113">Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens status for overholdelse.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="5a0fb-114">Rediger brugerens betingede adgangstildeling.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="5a0fb-115">I Azure-portalen skal du gå til Politikker for betinget adgang i **Intune.**  >    >  </span><span class="sxs-lookup"><span data-stu-id="5a0fb-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="5a0fb-116">Vælg en politik på listen.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="5a0fb-117">Klik på Brugere og grupper.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-117">Click Users and groups.</span></span>
4. <span data-ttu-id="5a0fb-118">Hvis du vil målrette en bestemt politik mod en person, kan du føje dem til listen Medtag.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="5a0fb-119">For at sikre, at en person udelades fra politikken, kan du føje dem til listen Udelad.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="5a0fb-120">Nyttige links:</span><span class="sxs-lookup"><span data-stu-id="5a0fb-120">Helpful links:</span></span>

[<span data-ttu-id="5a0fb-121">Oversigt over enhedsoverholdelse</span><span class="sxs-lookup"><span data-stu-id="5a0fb-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="5a0fb-122">Fejlfindings-nøglecenter</span><span class="sxs-lookup"><span data-stu-id="5a0fb-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="5a0fb-123">Fejlfindingspolitik</span><span class="sxs-lookup"><span data-stu-id="5a0fb-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="5a0fb-124">Overvågning af overholdelse af intune-enhed</span><span class="sxs-lookup"><span data-stu-id="5a0fb-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="5a0fb-125">Bemærk! Disse trin er kun nyttige ved fejlfinding af funktionen Betinget adgang til Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="5a0fb-126">Det er også muligt at sætte en enhed i karantæne, der blokerer dens mailadgang med Exchange-politik.</span><span class="sxs-lookup"><span data-stu-id="5a0fb-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="5a0fb-127">Du kan finde flere oplysninger om administration af exchange-enheder [her]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="5a0fb-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
