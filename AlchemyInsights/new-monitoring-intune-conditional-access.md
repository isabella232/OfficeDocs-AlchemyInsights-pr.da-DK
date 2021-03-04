---
title: Overvåg Betinget adgang i Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427428"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="bb2a4-102">Overvåg Betinget adgang i Intune</span><span class="sxs-lookup"><span data-stu-id="bb2a4-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="bb2a4-103">Brugere, der er målrettet betinget adgang, modtager en mail, hvis de ikke opfylder din organisations adgangskrav.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="bb2a4-104">For at løse dette anbefaler vi en eller flere af følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="bb2a4-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="bb2a4-105">Hvis enheden antages at være tilmeldt, skal du opfordre brugeren til at gå til appen Firmaportal og kontrollere, at den vises i firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="bb2a4-106">Hvis den ikke gør det, skal brugeren tilmelde enheden.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="bb2a4-107">I Azure-portalen skal du gå til **overholdelse af regler og standarder for Intune-enheder.**  >  </span><span class="sxs-lookup"><span data-stu-id="bb2a4-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="bb2a4-108">Hvis du vil have vist rapporten om overholdelse af regler og standarder for enheden for at bekræfte, at brugerens enhed er markeret som kompatibel, **skal** du klikke på Enhedsoverholdelse under **Skærm.**</span><span class="sxs-lookup"><span data-stu-id="bb2a4-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="bb2a4-109">I Azure-portalen skal du gå til **overholdelse af regler og standarder for Intune-enheder.**  >  </span><span class="sxs-lookup"><span data-stu-id="bb2a4-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="bb2a4-110">Klik **på Politikker** under **Administrer.**</span><span class="sxs-lookup"><span data-stu-id="bb2a4-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="bb2a4-111">Kontrollér, at der er tildelt en profil til brugerens enhed på listen over politikker for overholdelse af regler og standarder.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="bb2a4-112">Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens status for overholdelse.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="bb2a4-113">Rediger brugerens betingede adgangstildeling.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="bb2a4-114">I Azure-portalen skal du gå til Politikker for betinget adgang i **Intune,** vælge en politik på listen  >    >  og klikke **på Brugere og grupper.**</span><span class="sxs-lookup"><span data-stu-id="bb2a4-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="bb2a4-115">Hvis du vil målrette en bestemt politik mod en person, skal du føje dem **til listen Medtag.**</span><span class="sxs-lookup"><span data-stu-id="bb2a4-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="bb2a4-116">For at sikre, at en person udelades fra politikken, kan du føje dem til **listen Udelad.**</span><span class="sxs-lookup"><span data-stu-id="bb2a4-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="bb2a4-117">**Nyttige links:**</span><span class="sxs-lookup"><span data-stu-id="bb2a4-117">**Helpful links:**</span></span>

- [<span data-ttu-id="bb2a4-118">Oversigt over enhedsoverholdelse</span><span class="sxs-lookup"><span data-stu-id="bb2a4-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="bb2a4-119">Fejlfindings-nøglecenter</span><span class="sxs-lookup"><span data-stu-id="bb2a4-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="bb2a4-120">Fejlfindingspolitik</span><span class="sxs-lookup"><span data-stu-id="bb2a4-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="bb2a4-121">Overvågning af overholdelse af Intune-enhed</span><span class="sxs-lookup"><span data-stu-id="bb2a4-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="bb2a4-122">Disse trin er kun nyttige ved fejlfinding af Funktionen Betinget adgang til Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="bb2a4-123">Det er også muligt at sætte en enhed i karantæne, der blokerer dens mailadgang med Exchange-politik.</span><span class="sxs-lookup"><span data-stu-id="bb2a4-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="bb2a4-124">Du kan finde flere oplysninger om administration af enheder i Exchange [**her.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="bb2a4-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
