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
# <a name="pausing-scheduled-updates"></a>Midlertidig afbrydelse af planlagte opdateringer

Når der udstedes en pause-kommando, behandler enheder ikke kommandoen før næste gang, de tjekker ind til Intune. Derfor kan dine enheder have:

- Har installeret de planlagte opdateringer, før du tjekker ind.
- Blevet slukket, da du udstedte kommandoen pause. Hvis enhederne er tændt, kan de i dette tilfælde have downloadet og installeret de planlagte opdateringer, før du tjekker ind.