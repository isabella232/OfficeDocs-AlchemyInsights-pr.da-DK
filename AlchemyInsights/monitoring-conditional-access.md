---
title: Overvågning af betinget adgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713712"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="bc070-102">Overvågning af betinget adgang til Exchange</span><span class="sxs-lookup"><span data-stu-id="bc070-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="bc070-103">Brugere, der er målrettet mod betinget adgang, modtager en e-mail med en meddelelse, hvis de ikke opfylder organisationens adgangskrav.</span><span class="sxs-lookup"><span data-stu-id="bc070-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="bc070-104">Vi anbefaler en eller flere af følgende løsninger for at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="bc070-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="bc070-105">Hvis enheden formodes at være tilmeldt, skal du råde brugeren til at gå til appen Firmaportal og bekræfte, at den vises i virksomhedsportalen.</span><span class="sxs-lookup"><span data-stu-id="bc070-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="bc070-106">Hvis det ikke er tilfældet, skal brugeren tilmelde enheden.</span><span class="sxs-lookup"><span data-stu-id="bc070-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="bc070-107">I Azure-portalen skal du gå til **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="bc070-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bc070-108">Klik på **Enhedsoverholdelse af enhed**under **Skærm** .</span><span class="sxs-lookup"><span data-stu-id="bc070-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="bc070-109">Få vist rapporten om overholdelse af enheden for at kontrollere, at brugerens enhed er markeret som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="bc070-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="bc070-110">I Azure-portalen skal du gå til **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="bc070-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="bc070-111">Klik på **Politikker**under **Administrer**.</span><span class="sxs-lookup"><span data-stu-id="bc070-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="bc070-112">På listen over overholdelsespolitikker skal du kontrollere, at der er tildelt en profil til din brugers enhed.</span><span class="sxs-lookup"><span data-stu-id="bc070-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="bc070-113">Hvis der ikke er tildelt en profil, kan Intune ikke bekræfte enhedens overholdelsesstatus.</span><span class="sxs-lookup"><span data-stu-id="bc070-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="bc070-114">Rediger brugerens tildeling med betinget adgang.</span><span class="sxs-lookup"><span data-stu-id="bc070-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="bc070-115">På Azure-portalen skal du gå til **Intune-politikker \> for \> betinget adgang**</span><span class="sxs-lookup"><span data-stu-id="bc070-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="bc070-116">Vælg en politik på listen</span><span class="sxs-lookup"><span data-stu-id="bc070-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="bc070-117">Klik på **Brugere og grupper**</span><span class="sxs-lookup"><span data-stu-id="bc070-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="bc070-118">Hvis du vil målrette mod en bestemt politik mod en person, skal du føje dem til listen **Medtag.**</span><span class="sxs-lookup"><span data-stu-id="bc070-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="bc070-119">Hvis du vil sikre, at en person udelades fra politikken, skal du føje vedkommende til listen **Udeluk.**</span><span class="sxs-lookup"><span data-stu-id="bc070-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="bc070-120">Læs mere: [Sådan overvåges Betingede Access-enheder](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="bc070-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

