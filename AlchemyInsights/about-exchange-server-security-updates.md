---
title: Om Exchange Server sikkerhedsopdateringer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481118"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="dd42d-102">Om Exchange Server sikkerhedsopdateringer</span><span class="sxs-lookup"><span data-stu-id="dd42d-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="dd42d-103">Microsoft har udgivet en række vigtige sikkerhedsopdateringer til Exchange Server lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="dd42d-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="dd42d-104">De påvirkede serverversioner er alle opdateringsniveauer i Exchange Server 2010, 2013, 2016 og 2019.</span><span class="sxs-lookup"><span data-stu-id="dd42d-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="dd42d-105">Exchange Online påvirkes IKKE, men hvis du har nogle lokale Exchange-servere på grund af hybridkonfiguration, er de potentielt sårbar.</span><span class="sxs-lookup"><span data-stu-id="dd42d-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="dd42d-106">Hvis du vil opdatere dine lokale servere, skal der som minimum køres følgende versioner af Exchange:</span><span class="sxs-lookup"><span data-stu-id="dd42d-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="dd42d-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="dd42d-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="dd42d-108">Exchange Server 23 CU 2013</span><span class="sxs-lookup"><span data-stu-id="dd42d-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="dd42d-109">Exchange Server 2016 CU 19 eller CU 18</span><span class="sxs-lookup"><span data-stu-id="dd42d-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="dd42d-110">Exchange Server 2019 CU 8 eller CU 7</span><span class="sxs-lookup"><span data-stu-id="dd42d-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="dd42d-111">Se følgende meddelelse om placering af rettelser: [Udgivet: Marts 2021 Exchange Server sikkerhedsopdateringer](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="dd42d-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="dd42d-112">**Vigtige bemærkninger:**</span><span class="sxs-lookup"><span data-stu-id="dd42d-112">**Important notes:**</span></span>

<span data-ttu-id="dd42d-113">Installation af opdateringer fungerer ikke, hvis dine lokale servere ikke kører nødvendige Exchange-versioner, som vist på listen ovenfor.</span><span class="sxs-lookup"><span data-stu-id="dd42d-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="dd42d-114">Hvis du installerer opdateringer manuelt, skal du læse afsnittet "Kendte problemer" i artiklerne om opdatering af KB for at få vigtige oplysninger.</span><span class="sxs-lookup"><span data-stu-id="dd42d-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="dd42d-115">Sikkerhedsopdateringer SKAL køres fra administratorerede CMD/PowerShell-prompts!</span><span class="sxs-lookup"><span data-stu-id="dd42d-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
