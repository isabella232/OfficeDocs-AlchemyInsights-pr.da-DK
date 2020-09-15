---
title: Sådan deaktiveres eksterne grupper
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704122"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="83c10-102">Sådan deaktiveres eksterne grupper</span><span class="sxs-lookup"><span data-stu-id="83c10-102">How to disable External Groups</span></span>

<span data-ttu-id="83c10-103">Yammer-ekstern kommunikation anvender regler for Exchange-transport (Etr'er), et sæt proaktive kontrolelementer til at forhindre, at firmaoplysninger deles.</span><span class="sxs-lookup"><span data-stu-id="83c10-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="83c10-104">Hvis du vil begrænse brugerne i at oprette eksterne grupper, skal du konfigurere en Exchange-transportregel (ETR) og derefter konfigurere Yammer til at blokere for eksterne meddelelser.</span><span class="sxs-lookup"><span data-stu-id="83c10-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="83c10-105">Når du har oprettet en regel i Exchange Online Administration, skal du følge disse trin for at angive ETR, der skal anvendes i Yammer:</span><span class="sxs-lookup"><span data-stu-id="83c10-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="83c10-106">Log på Yammer som en bekræftet administrator, og gå til **yammer-Administrationscenter**og gå til C **indhold og sikkerhedsindstillinger for sikkerhed \> .**</span><span class="sxs-lookup"><span data-stu-id="83c10-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="83c10-107">Gå til **eksterne meddelelser**, og vælg **Gennemtving dine Exchange Online Exchange-transport regler (Etr'er) i Yammer.**</span><span class="sxs-lookup"><span data-stu-id="83c10-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="83c10-108">Vælg **Gem**.</span><span class="sxs-lookup"><span data-stu-id="83c10-108">Choose **Save**.</span></span>

<span data-ttu-id="83c10-109">Hvis du vil have mere at vide, skal du se [Deaktiver eksterne beskeder i et Yammer-netværk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="83c10-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  