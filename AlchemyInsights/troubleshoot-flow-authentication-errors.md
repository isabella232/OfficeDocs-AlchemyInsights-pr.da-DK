---
title: Fejlfinding af flow-godkendelsesfejl
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690561"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="7fbe0-102">Fejlfinding af flow-godkendelsesfejl</span><span class="sxs-lookup"><span data-stu-id="7fbe0-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="7fbe0-103">I mange tilfælde mislykkes flows på grund af en godkendelsesfejl.</span><span class="sxs-lookup"><span data-stu-id="7fbe0-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="7fbe0-104">Hvis du har denne type fejl, indeholder fejlmeddelelsen "uautoriseret", eller der vises en fejlkode på 401 eller 403.</span><span class="sxs-lookup"><span data-stu-id="7fbe0-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="7fbe0-105">Du kan som regel rette en godkendelsesfejl ved at opdatere forbindelsen:</span><span class="sxs-lookup"><span data-stu-id="7fbe0-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="7fbe0-106">Øverst på webportalen skal du klikke eller trykke på gear-ikonet for at åbne menuen Indstillinger og derefter klikke eller trykke på **forbindelser**.</span><span class="sxs-lookup"><span data-stu-id="7fbe0-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="7fbe0-107">Rul ned til den forbindelse, du har set den uautoriserede fejlmeddelelse for.</span><span class="sxs-lookup"><span data-stu-id="7fbe0-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="7fbe0-108">Klik eller tryk på linket **Bekræft adgangskode** ud for forbindelsen, og klik på den meddelelse om forbindelsen, der ikke er godkendt.</span><span class="sxs-lookup"><span data-stu-id="7fbe0-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="7fbe0-109">Bekræft dine legitimationsoplysninger ved at følge instruktionerne, der vises, gå tilbage til din flow-kørselsfejl, og klik eller tryk derefter på **Gensend**.</span><span class="sxs-lookup"><span data-stu-id="7fbe0-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="7fbe0-110">Hvis du vil have mere hjælp, skal du se [fejlfinding i et flow](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="7fbe0-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

