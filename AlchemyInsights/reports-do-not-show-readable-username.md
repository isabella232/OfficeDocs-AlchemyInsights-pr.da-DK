---
title: Rapporter i Microsoft 365 Administration viser ikke læsbart brugernavn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2021
ms.locfileid: "59315871"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Rapporter i Microsoft 365 Administration viser ikke læsbart brugernavn

Rapporter i Microsoft 365 Administration ikke brugernavne, men viser i stedet alfanumeriske værdier som f.eks. B2BC6C15BB9FCDEA71E5CD302D228CC8.

Dette er den forventede funktionsmåde og er blevet meddelt i Meddelelsescenter (MC275344, publiceret 3. august 2021). 

Globale administratorer kan vende tilbage til denne ændring for deres lejer og vise identificerbare brugeroplysninger, hvis organisationens praksis for beskyttelse af personlige oplysninger tillader det. Sådan gendannes ændringen for lejeren:

1. I Administration skal du gå til **Indstillinger**  >  **Org settings**  >  [**Services**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)og vælge **Rapporter**. 
1. Under **Vælg, hvordan brugeroplysninger skal vises** skal du vælge Vis **identificerbare brugeroplysninger i** rapporter og derefter køre rapporten igen.