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
# <a name="pausing-scheduled-updates"></a>Sætte planlagte opdateringer på pause

Når der udstedes en pausekommando, behandler enhederne ikke kommandoen, før de tjekker ind på Intune, næste gang de tjekker ind på Intune. På grund af dette kan dine enheder have:

- Har installeret de planlagte opdateringer før indtjekning.
- Blevet slukket, da du udstedte pausekommandoen. I dette tilfælde, når enhederne blev tændt, kunne de have downloadet og installeret de planlagte opdateringer før check-in.