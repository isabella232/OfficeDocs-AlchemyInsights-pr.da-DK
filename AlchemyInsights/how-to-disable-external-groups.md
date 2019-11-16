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
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36739487"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="fc74c-102">Sådan deaktiveres eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="fc74c-102">How to disable External Groups</span></span>

<span data-ttu-id="fc74c-103">Yammer External messaging anvender Exchange transport Rules (ETRs), et sæt proaktive kontrolelementer for at forhindre, at virksomhedsoplysninger deles.</span><span class="sxs-lookup"><span data-stu-id="fc74c-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="fc74c-104">Hvis du vil begrænse brugere i at oprette eksterne grupper, skal du konfigurere en Exchange transport Rule (ETR) og derefter konfigurere Yammer til at bruge Exchange-transportreglen til at blokere eksterne meddelelser.</span><span class="sxs-lookup"><span data-stu-id="fc74c-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="fc74c-105">Når du har oprettet en regel i Exchange Online Administration, skal du følge disse trin for at indstille ETR til at gælde i Yammer:</span><span class="sxs-lookup"><span data-stu-id="fc74c-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="fc74c-106">Log på Yammer som en bekræftet administrator, og gå til indstillinger for C- **indhold og sikkerheds \> sikkerhed** i **yammer administration**.</span><span class="sxs-lookup"><span data-stu-id="fc74c-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="fc74c-107">Under **eksterne meddelelser**skal du vælge gennem **Tving dine Exchange Online Exchange transport Rules (ETRS) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="fc74c-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="fc74c-108">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="fc74c-108">Choose **Save**.</span></span>

<span data-ttu-id="fc74c-109">Du finder flere oplysninger under [deaktivere eksterne meddelelser i et Yammer-netværk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="fc74c-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  