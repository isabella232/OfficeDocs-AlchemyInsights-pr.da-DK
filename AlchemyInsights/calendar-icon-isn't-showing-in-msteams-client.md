---
title: Kalenderikonet vises ikke i Microsoft teams-klienten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583344"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Kalenderikonet vises ikke i Microsoft teams-klienten

Fanen **kalender** i teams kræver adgang til en Exchange-postkasse via Exchange-Webtjenester. Exchange-postkassen kan være online eller lokalt. For online brugere, der ikke kan se fanen **kalender** , skal du kontrollere, at de [er givet i licens til en Exchange Online-postkasse, og at postkassen er aktiveret](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Hvis dine brugere har hjem lokalt, skal du bekræfte, at din hybrid konfiguration er i orden. Brug [Guiden Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) til fejlfinding. Bemærk, at [Teams kræver Exchange 2016 CU3 eller højere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Du kan finde flere oplysninger og fejlfindingstrin under [fejlfinding af problemer med Microsoft teams og Exchange Server-samspil](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
