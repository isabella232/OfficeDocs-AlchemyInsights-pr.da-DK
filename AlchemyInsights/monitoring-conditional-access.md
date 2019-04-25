---
title: Overvågning af adgangsstyring
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418463"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="8f8c9-102">Overvågning af adgangsstyring</span><span class="sxs-lookup"><span data-stu-id="8f8c9-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="8f8c9-103">Brugere, der er målrettet med adgangsstyring modtager en besked via e-mail, hvis de ikke opfylder adgangskravene til din organisation.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="8f8c9-104">Du kan løse, anbefaler vi en eller flere af følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="8f8c9-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="8f8c9-105">Hvis enheden antages at være tilmeldt, oplyse brugeren om at gå til firmaets Portal-app, og Kontroller, at det vises i firmaets Portal.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="8f8c9-106">Hvis det ikke er tilfældet, skal brugeren registrere enheden.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="8f8c9-107">Gå til portalen Azure **Intune \> enhed overholdelse af**.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="8f8c9-108">Klik på **enhed overholdelse**under **skærm** .</span><span class="sxs-lookup"><span data-stu-id="8f8c9-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="8f8c9-109">Få vist rapporten til at kontrollere, at brugerens enhed er markeret som værende kompatibel enhed overholdes.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="8f8c9-110">Gå til portalen Azure **Intune \> enhed overholdelse af**.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="8f8c9-111">Klik på **politikker**under **Administrer**.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="8f8c9-112">Kontroller, der er tildelt en profil til brugerens enhed på listen over overholdelse af politikker.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="8f8c9-113">Hvis der er tildelt nogen profil, derefter kunne Intune ikke bekræfte enhedens overholdelsesstatus.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="8f8c9-114">Rediger brugerens adgangsstyring tildeling.</span><span class="sxs-lookup"><span data-stu-id="8f8c9-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="8f8c9-115">Gå til portalen Azure **Intune \> adgangsstyring \> politikker for**</span><span class="sxs-lookup"><span data-stu-id="8f8c9-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="8f8c9-116">Vælg en politik på listen</span><span class="sxs-lookup"><span data-stu-id="8f8c9-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="8f8c9-117">Klik på **brugere og grupper**</span><span class="sxs-lookup"><span data-stu-id="8f8c9-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="8f8c9-118">Hvis du vil målrette en bestemt politik på en person, kan du tilføje dem på **listen** .</span><span class="sxs-lookup"><span data-stu-id="8f8c9-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="8f8c9-119">For at sikre, at en person, der er udeladt fra politikken, kan du føje dem til listen **udelades** .</span><span class="sxs-lookup"><span data-stu-id="8f8c9-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="8f8c9-120">Læs mere: [Sådan skærm adgangsstyring enheder](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="8f8c9-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

