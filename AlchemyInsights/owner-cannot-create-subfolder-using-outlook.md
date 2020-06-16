---
title: Ejeren kan ikke oprette undermappe ved hjælp af Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748790"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ejeren kan ikke oprette undermappe ved hjælp af Outlook

**Der er et vedvarende problem med ejere af offentlige mapper, der opretter undermapper ved hjælp af Outlook. Problemet vil blive løst snart.**

Brug i mellemtiden en af følgende løsninger:

1. Brug Outlook til MAC til at oprette undermappen, da problemet kun påvirker Outlook til skrivebordsvinduer (alle versioner)
2. Få administratoren til at oprette undermappen ved hjælp af EXO Shell eller EAC
3. Ændre standardpostublicFolderMailbox/EffectivePublicFolderMailbox på brugeren til en anden postkasse end indholdspostkassen for den mappe, der forårsager problemet  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Vent i en time, genstart Outlook-klienten