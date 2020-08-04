---
title: Sætte planlagte opdateringer på pause
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555103"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="c7c92-102">Sætte planlagte opdateringer på pause</span><span class="sxs-lookup"><span data-stu-id="c7c92-102">Pausing scheduled updates</span></span>

<span data-ttu-id="c7c92-103">Når der udstedes en pausekommando, behandler enhederne ikke kommandoen, før de tjekker ind på Intune, næste gang de tjekker ind på Intune.</span><span class="sxs-lookup"><span data-stu-id="c7c92-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="c7c92-104">På grund af dette kan dine enheder have:</span><span class="sxs-lookup"><span data-stu-id="c7c92-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="c7c92-105">Har installeret de planlagte opdateringer før indtjekning.</span><span class="sxs-lookup"><span data-stu-id="c7c92-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="c7c92-106">Blevet slukket, da du udstedte pausekommandoen.</span><span class="sxs-lookup"><span data-stu-id="c7c92-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="c7c92-107">I dette tilfælde, når enhederne blev tændt, kunne de have downloadet og installeret de planlagte opdateringer før check-in.</span><span class="sxs-lookup"><span data-stu-id="c7c92-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>