---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720762"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="3c27f-102">Sådan deaktiveres eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="3c27f-102">How to disable External Groups</span></span>

<span data-ttu-id="3c27f-103">Yammers eksterne meddelelser anvender Exchange Transport Rules (ETR'er), som er et sæt proaktive kontrolelementer, der forhindrer, at virksomhedsoplysninger deles.</span><span class="sxs-lookup"><span data-stu-id="3c27f-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="3c27f-104">Hvis du vil begrænse brugeres mulighed for at oprette eksterne grupper, skal du konfigurere en Exchange-transportregel (ETR) og derefter konfigurere Yammer til at bruge Exchange Transport-reglen til at blokere eksterne meddelelser.</span><span class="sxs-lookup"><span data-stu-id="3c27f-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="3c27f-105">Når du har oprettet en regel i Exchange Online Administration, skal du følge disse trin for at indstille ETR til at gælde i Yammer:</span><span class="sxs-lookup"><span data-stu-id="3c27f-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="3c27f-106">Log på Yammer som en bekræftet administrator, og gå til **C-indstillinger \> for indholds- og sikkerhedssikkerhed i** **Yammer Administration.**</span><span class="sxs-lookup"><span data-stu-id="3c27f-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="3c27f-107">Vælg **Gennemtving dine Exchange Online Exchange Transport-regler (ETR'er) i Yammer under** **Eksterne meddelelser.**</span><span class="sxs-lookup"><span data-stu-id="3c27f-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="3c27f-108">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="3c27f-108">Choose **Save**.</span></span>

<span data-ttu-id="3c27f-109">Yderligere oplysninger finder du i [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="3c27f-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  