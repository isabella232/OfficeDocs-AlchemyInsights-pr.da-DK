---
title: Ejeren kan ikke oprette en undermappe ved hjælp af Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836129"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ejeren kan ikke oprette en undermappe ved hjælp af Outlook

**Der er i øjeblikket et problem med ejere af offentlige mapper, der opretter undermapper ved hjælp af Outlook. Problemet vil snart blive rettet.**

I mellemtiden kan du bruge en af følgende løsninger:

1. Brug Outlook til MAC til at oprette undermappen, da problemet kun påvirker Outlook til skrivebordsvinduer (alle versioner)
2. Få administratoren til at oprette undermappen ved hjælp af EXO Shell eller EAC
3. Skift DefaultPublicFolderMailbox/EffectivePublicFolderMailbox på brugeren til en anden postkasse end indholdspostkassen for mappen, der forårsager problemer  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Vent en time, genstart Outlook-klienten