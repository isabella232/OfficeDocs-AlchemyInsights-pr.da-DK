---
title: Kan ikke få adgang til offentlige mapper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959489"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke oprette forbindelse til offentlige mapper

Hvis adgang til offentlige mapper ikke fungerer for få brugere, kan du prøve følgende:

Opret forbindelse til EXO PowerShell, og Konfigurer DefaultPublicFolderMailbox på den problematiske brugerkonto, så den svarer til en på en fungerende brugerkonto.

Eksempel:

Hent-postkasse WorkingUser | ft DefaultPublicFolderMailbox, Effekvepublicfoldermailbox

Set-postkasse Problembruger-DefaultPublicFolderMailbox \<Value fra forrige kommando>

Vent mindst en time, indtil ændringen træder i kraft.