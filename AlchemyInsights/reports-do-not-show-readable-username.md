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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327808"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Rapporter i Microsoft 365 Administration viser ikke læsbart brugernavn

Rapporter i Microsoft 365 Administration viser ikke brugernavne, men viser i stedet alfanumeriske værdier som B2BC6C15BB9FCDEA71E5CD302D228CC8.

Dette er den forventede adfærd og er blevet meddelt i Meddelelsescenter (MC275344, udgivet 3. august 2021). 

Globale administratorer kan annullere denne ændring for deres lejer og vise identificerbare brugeroplysninger, hvis organisationens praksis for beskyttelse af personlige oplysninger tillader det. Sådan annullerer du ændringen for lejeren:

1. I Administration skal du gå til **Indstillinger** > **Organisationsindstillinger** > [**Tjenester**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) og vælge **Rapporter**. 
1. Under **Vælg, hvordan brugeroplysninger vises** skal du vælge **Vis identificerbare brugeroplysninger i rapporter** og derefter køre rapporten igen.