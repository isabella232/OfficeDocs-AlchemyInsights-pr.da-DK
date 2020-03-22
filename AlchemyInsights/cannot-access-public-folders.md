---
title: Der kan ikke få adgang til offentlige mapper
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891743"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke oprette forbindelse til offentlige mapper

Hvis adgang til offentlige mapper ikke fungerer for nogle brugere, kan du prøve følgende:

Opret forbindelse til EXO PowerShell, og konfigurer parameteren DefaultPublicFolderMailbox på problembrugerkontoen, så den svarer til parameteren på en fungerende brugerkonto.

Eksempel:

Arbejdsbruger til hent postkasse | ft DefaultPublicFolderMailbox,EffektivPublicFolderMailbox

Set-Mailbox ProblemBruger -DefaultPublicFolderMailbox-værdi \<fra tidligere kommando>

Vent mindst en time, før ændringen træder i kraft.

Hvis problemet stadig er, skal du følge [denne fremgangsmåde](https://aka.ms/pfcte) for at foretage fejlfinding af problemer med adgang til offentlige mapper ved hjælp af Outlook.