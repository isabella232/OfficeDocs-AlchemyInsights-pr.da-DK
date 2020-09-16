---
title: Midlertidig afbrydelse af planlagte opdateringer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721549"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="5e033-102">Midlertidig afbrydelse af planlagte opdateringer</span><span class="sxs-lookup"><span data-stu-id="5e033-102">Pausing scheduled updates</span></span>

<span data-ttu-id="5e033-103">Når der udstedes en pause-kommando, behandler enheder ikke kommandoen før næste gang, de tjekker ind til Intune.</span><span class="sxs-lookup"><span data-stu-id="5e033-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="5e033-104">Derfor kan dine enheder have:</span><span class="sxs-lookup"><span data-stu-id="5e033-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="5e033-105">Har installeret de planlagte opdateringer, før du tjekker ind.</span><span class="sxs-lookup"><span data-stu-id="5e033-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="5e033-106">Blevet slukket, da du udstedte kommandoen pause.</span><span class="sxs-lookup"><span data-stu-id="5e033-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="5e033-107">Hvis enhederne er tændt, kan de i dette tilfælde have downloadet og installeret de planlagte opdateringer, før du tjekker ind.</span><span class="sxs-lookup"><span data-stu-id="5e033-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>