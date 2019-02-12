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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902335"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="a0277-102">Overvågning af adgangsstyring</span><span class="sxs-lookup"><span data-stu-id="a0277-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="a0277-p101">Brugere, der er målrettet med adgangsstyring modtager en besked via e-mail, hvis de ikke opfylder adgangskravene til din organisation. Du kan løse, anbefaler vi en eller flere af følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="a0277-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a0277-p102">Hvis enheden antages at være tilmeldt, oplyse brugeren om at gå til firmaets Portal-app, og Kontroller, at det vises i firmaets Portal. Hvis det ikke er tilfældet, skal brugeren registrere enheden.</span><span class="sxs-lookup"><span data-stu-id="a0277-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a0277-p103">Gå til portalen Azure **Intune \> enhed overholdelse af**. Klik på **enhed overholdelse**under **skærm** . Få vist rapporten til at kontrollere, at brugerens enhed er markeret som værende kompatibel enhed overholdes.</span><span class="sxs-lookup"><span data-stu-id="a0277-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a0277-p104">Gå til portalen Azure **Intune \> enhed overholdelse af**. Klik på **politikker**under **Administrer**. Kontroller, der er tildelt en profil til brugerens enhed på listen over overholdelse af politikker. Hvis der er tildelt nogen profil, derefter kunne Intune ikke bekræfte enhedens overholdelsesstatus.</span><span class="sxs-lookup"><span data-stu-id="a0277-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a0277-114">Rediger brugerens adgangsstyring tildeling.</span><span class="sxs-lookup"><span data-stu-id="a0277-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a0277-115">Gå til portalen Azure **Intune \> adgangsstyring \> politikker for**</span><span class="sxs-lookup"><span data-stu-id="a0277-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a0277-116">Vælg en politik på listen</span><span class="sxs-lookup"><span data-stu-id="a0277-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a0277-117">Klik på **brugere og grupper**</span><span class="sxs-lookup"><span data-stu-id="a0277-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a0277-p105">Hvis du vil målrette en bestemt politik på en person, kan du tilføje dem på **listen** . For at sikre, at en person, der er udeladt fra politikken, kan du føje dem til listen **udelades** .</span><span class="sxs-lookup"><span data-stu-id="a0277-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a0277-120">Læs mere: [Sådan skærm adgangsstyring enheder](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a0277-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

