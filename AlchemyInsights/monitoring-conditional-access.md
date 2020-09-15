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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702897"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a76fa-102">Overvågning af betinget adgang for Exchange</span><span class="sxs-lookup"><span data-stu-id="a76fa-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a76fa-103">Brugere, der er målrettet med betinget adgang, modtager en mailbesked, hvis de ikke opfylder din organisations adgangs krav.</span><span class="sxs-lookup"><span data-stu-id="a76fa-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a76fa-104">Vi anbefaler en eller flere af følgende løsninger for at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="a76fa-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a76fa-105">Hvis enheden anses for at være tilmeldt, skal du bede brugeren om at gå til appen Firmaportal og bekræfte, at den vises på Firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="a76fa-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a76fa-106">Hvis det ikke er den, skal brugeren tilmelde enheden.</span><span class="sxs-lookup"><span data-stu-id="a76fa-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a76fa-107">I Azure-portalen skal du gå til **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="a76fa-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a76fa-108">Klik på **enheds overholdelse**under **overvågning** .</span><span class="sxs-lookup"><span data-stu-id="a76fa-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="a76fa-109">Se din enheds kompatibilitetsrapport for at bekræfte, at brugerens enhed er markeret som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="a76fa-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a76fa-110">I Azure-portalen skal du gå til **Intune \> Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="a76fa-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="a76fa-111">Under **Administrer**skal du klikke på **politikker**.</span><span class="sxs-lookup"><span data-stu-id="a76fa-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="a76fa-112">På listen over overholdelsespolitikker skal du kontrollere, at der er tildelt en profil til din brugers enhed.</span><span class="sxs-lookup"><span data-stu-id="a76fa-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a76fa-113">Hvis der ikke er tildelt nogen profil, vil Intune ikke kunne bekræfte enhedens overholdelses status.</span><span class="sxs-lookup"><span data-stu-id="a76fa-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a76fa-114">Redigere brugerens betingede adgangs tildeling.</span><span class="sxs-lookup"><span data-stu-id="a76fa-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a76fa-115">I Azure-portalen skal du gå til \*\* \> \> politikker for betinget adgang til Intune\*\*</span><span class="sxs-lookup"><span data-stu-id="a76fa-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a76fa-116">Vælg en politik på listen</span><span class="sxs-lookup"><span data-stu-id="a76fa-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a76fa-117">Klik på **brugere og grupper**</span><span class="sxs-lookup"><span data-stu-id="a76fa-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a76fa-118">Hvis du vil målrette en bestemt politik til en anden, skal du føje dem til listen **Medtag** .</span><span class="sxs-lookup"><span data-stu-id="a76fa-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="a76fa-119">Hvis du vil sikre dig, at en person udelades fra politikken, skal du føje dem til listen **Udelad** .</span><span class="sxs-lookup"><span data-stu-id="a76fa-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a76fa-120">Læs mere: [Sådan overvåges enheder med betinget adgang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a76fa-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

