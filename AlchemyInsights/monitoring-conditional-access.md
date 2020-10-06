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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366422"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="d69e0-102">Overvågning af betinget adgang for Exchange</span><span class="sxs-lookup"><span data-stu-id="d69e0-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="d69e0-103">Brugere, der er målrettet med betinget adgang, modtager en mailbesked, hvis de ikke opfylder din organisations adgangs krav.</span><span class="sxs-lookup"><span data-stu-id="d69e0-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="d69e0-104">Vi anbefaler en eller flere af følgende løsninger for at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="d69e0-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="d69e0-105">Hvis enheden anses for at være tilmeldt, skal du bede brugeren om at gå til appen Firmaportal og bekræfte, at den vises på Firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="d69e0-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="d69e0-106">Hvis det ikke er den, skal brugeren tilmelde enheden.</span><span class="sxs-lookup"><span data-stu-id="d69e0-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="d69e0-107">I Azure-portalen skal du gå til Intune > enhedskompatibilitet.</span><span class="sxs-lookup"><span data-stu-id="d69e0-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="d69e0-108">Klik på enheds overholdelse under overvågning.</span><span class="sxs-lookup"><span data-stu-id="d69e0-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="d69e0-109">Se din enheds kompatibilitetsrapport for at bekræfte, at brugerens enhed er markeret som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="d69e0-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="d69e0-110">I Azure-portalen skal du gå til Intune > enhedskompatibilitet.</span><span class="sxs-lookup"><span data-stu-id="d69e0-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="d69e0-111">Under Administrer skal du klikke på politikker.</span><span class="sxs-lookup"><span data-stu-id="d69e0-111">Under Manage, click Policies.</span></span> <span data-ttu-id="d69e0-112">På listen over overholdelsespolitikker skal du kontrollere, at der er tildelt en profil til din brugers enhed.</span><span class="sxs-lookup"><span data-stu-id="d69e0-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="d69e0-113">Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens overholdelses status.</span><span class="sxs-lookup"><span data-stu-id="d69e0-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="d69e0-114">Redigere brugerens betingede adgangs tildeling.</span><span class="sxs-lookup"><span data-stu-id="d69e0-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="d69e0-115">Gå til politikker for **Intune**  >  **betinget adgang**til Intune i Azure-portalen  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="d69e0-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="d69e0-116">Vælg en politik på listen.</span><span class="sxs-lookup"><span data-stu-id="d69e0-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="d69e0-117">Klik på brugere og grupper.</span><span class="sxs-lookup"><span data-stu-id="d69e0-117">Click Users and groups.</span></span>
4. <span data-ttu-id="d69e0-118">Hvis du vil målrette en bestemt politik til en anden, skal du føje dem til listen Medtag.</span><span class="sxs-lookup"><span data-stu-id="d69e0-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="d69e0-119">Hvis du vil sikre dig, at en person udelades fra politikken, skal du føje dem til listen Udelad.</span><span class="sxs-lookup"><span data-stu-id="d69e0-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="d69e0-120">Nyttige links:</span><span class="sxs-lookup"><span data-stu-id="d69e0-120">Helpful links:</span></span>

[<span data-ttu-id="d69e0-121">Oversigt over enheds overholdelse</span><span class="sxs-lookup"><span data-stu-id="d69e0-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="d69e0-122">Fejlfindings NØGLECENTER</span><span class="sxs-lookup"><span data-stu-id="d69e0-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d69e0-123">Fejlfindings politik</span><span class="sxs-lookup"><span data-stu-id="d69e0-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="d69e0-124">Overvåge Intune-enhedskompatibilitet</span><span class="sxs-lookup"><span data-stu-id="d69e0-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="d69e0-125">Bemærk! disse trin er kun nyttige til fejlfinding af betinget adgang til Azure Active Directory-funktionen.</span><span class="sxs-lookup"><span data-stu-id="d69e0-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="d69e0-126">Det er også muligt at sætte en enheds blokering for en enhed, at det er en mail adgang med Exchange-politik.</span><span class="sxs-lookup"><span data-stu-id="d69e0-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="d69e0-127">Du kan finde flere oplysninger om administration af Exchange-enheder [her](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="d69e0-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
