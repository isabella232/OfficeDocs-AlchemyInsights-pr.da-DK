---
title: Ejeren kan ikke oprette en undermappe ved hjælp af Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665712"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Ejeren kan ikke oprette en undermappe ved hjælp af Outlook

**Der er et vedvarende problem med ejere af offentlige mapper, som opretter undermapper ved hjælp af Outlook. Problemet kan snart rettes.**

I mellemtiden kan du bruge en af følgende løsninger:

1. Brug Outlook til MAC til at oprette under mappen som et problem påvirker kun Outlook til stationære Windows (alle versioner)
2. Få administratoren til at oprette under mappen ved hjælp af EXO shell eller EAC
3. Ændre DefaultPublicFolderMailbox/EffectivePublicFolderMailbox på brugeren til en anden postkasse end indholds postkassen for mappen årsag til problemet  
    - *Set-postkasse User1 DefaultPublicFolderMailbox PubMBX3*
4. Vent en time, Genstart Outlook-klient