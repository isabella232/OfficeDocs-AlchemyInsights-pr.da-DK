---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28282504"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="49a96-102">Sådan deaktiveres eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="49a96-102">How to disable External Groups</span></span>

<span data-ttu-id="49a96-p101">Yammer eksterne meddelelser gælder Transport udvekslingsregler (ETRs), en række proaktive kontrol for at forhindre, at virksomhedens oplysninger deles. Hvis du vil forhindre brugere i at oprette eksterne grupper, skal du konfigurere en Exchange-transport regel (ETR), og konfigurer derefter Yammer for at bruge reglen Exchange Transport til at blokere eksterne meddelelser.</span><span class="sxs-lookup"><span data-stu-id="49a96-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="49a96-105">Når du har oprettet en regel i Exchange Online admin center, skal du følge disse trin for at angive ETR til anvendelse i Yammer:</span><span class="sxs-lookup"><span data-stu-id="49a96-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="49a96-106">Logge på Yammer som en kontrolleret admin, og i den **Yammer admin center**, skal du gå til C **Kræv og sikkerhed \> sikkerhedsindstillinger.**</span><span class="sxs-lookup"><span data-stu-id="49a96-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="49a96-107">Vælg under **Eksterne meddelelser**, **gennemtvinge din Exchange Online Transport udvekslingsregler (ETRs) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="49a96-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="49a96-108">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="49a96-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="49a96-109">Yderligere oplysninger finder du under [kontrol, der er eksterne meddelelser i et Yammer-netværk med regler for Transport af Exchange](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="49a96-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

