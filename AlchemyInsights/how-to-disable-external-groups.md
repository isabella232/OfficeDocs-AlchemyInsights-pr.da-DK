---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384819"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="115ab-102">Sådan deaktiveres eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="115ab-102">How to disable External Groups</span></span>

<span data-ttu-id="115ab-103">Yammer eksterne meddelelser gælder Transport udvekslingsregler (ETRs), en række proaktive kontrol for at forhindre, at virksomhedens oplysninger deles.</span><span class="sxs-lookup"><span data-stu-id="115ab-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="115ab-104">Hvis du vil forhindre brugere i at oprette eksterne grupper, skal du konfigurere en Exchange-transport regel (ETR), og konfigurer derefter Yammer for at bruge reglen Exchange Transport til at blokere eksterne meddelelser.</span><span class="sxs-lookup"><span data-stu-id="115ab-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="115ab-105">Når du har oprettet en regel i Exchange Online admin center, skal du følge disse trin for at angive ETR til anvendelse i Yammer:</span><span class="sxs-lookup"><span data-stu-id="115ab-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="115ab-106">Logge på Yammer som en kontrolleret admin, og i den **Yammer admin center**, skal du gå til C **indhold og sikkerhed \> sikkerhedsindstillinger.**</span><span class="sxs-lookup"><span data-stu-id="115ab-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="115ab-107">Vælg under **Eksterne meddelelser**, **gennemtvinge din Exchange Online Transport udvekslingsregler (ETRs) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="115ab-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="115ab-108">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="115ab-108">Choose **Save**.</span></span>

<span data-ttu-id="115ab-109">Yderligere oplysninger finder du under [kontrol, der er eksterne meddelelser i et Yammer-netværk med regler for Transport af Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="115ab-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  