---
title: Fejlfinding i forbindelse med flowgodkendelsesfejl
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 70451f074a65a4454faeadd188a31783be8e6c7e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759722"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="3ef08-102">Fejlfinding i forbindelse med flowgodkendelsesfejl</span><span class="sxs-lookup"><span data-stu-id="3ef08-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="3ef08-103">I mange tilfælde mislykkes flows på grund af en godkendelsesfejl.</span><span class="sxs-lookup"><span data-stu-id="3ef08-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="3ef08-104">Hvis du har denne type fejl, vises fejlmeddelelsen "Uautoriseret", eller der vises en fejlkode på 401 eller 403.</span><span class="sxs-lookup"><span data-stu-id="3ef08-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="3ef08-105">Du kan normalt rette en godkendelsesfejl ved at opdatere forbindelsen:</span><span class="sxs-lookup"><span data-stu-id="3ef08-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="3ef08-106">Klik eller tryk på **tandhjulsikonet**øverst på webportalen for at åbne menuen Indstillinger, og klik eller tryk derefter på Forbindelser .</span><span class="sxs-lookup"><span data-stu-id="3ef08-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="3ef08-107">Rul til den forbindelse, hvor du så fejlmeddelelsen Uautoriseret.</span><span class="sxs-lookup"><span data-stu-id="3ef08-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="3ef08-108">Klik eller tryk på linket **Bekræft adgangskode** i meddelelsen om, at forbindelsen ikke godkendes.</span><span class="sxs-lookup"><span data-stu-id="3ef08-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="3ef08-109">Bekræft dine legitimationsoplysninger ved at følge de instruktioner, der vises, vende tilbage til flow-run-fejlen, og klik eller tryk derefter på **Gensend igen**.</span><span class="sxs-lookup"><span data-stu-id="3ef08-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="3ef08-110">Du kan finde mere hjælp under [Fejlfinding af et flow](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="3ef08-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

