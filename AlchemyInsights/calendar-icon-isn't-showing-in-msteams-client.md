---
title: Kalenderikonet vises ikke i Microsoft Teams klient
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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54119998"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Kalenderikonet vises ikke i Microsoft Teams klient

Fanen **Kalender** i Teams kræver adgang til en Exchange via Exchange Web Services. Postkassen Exchange være Online eller Lokal. Onlinebrugere, der ikke  kan se fanen Kalender, skal kontrollere, at de har licens til en [Exchange Online, og at postkassen er aktiveret.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Hvis dine brugere er lokale brugere, skal du bekræfte, at din hybridkonfiguration er sund. Brug [Guiden Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) til fejlfinding. Bemærk, at [Teams kræver Exchange 2016 CU3 eller højere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Du kan finde flere oplysninger og fejlfindingstrin [under Fejlfinding Microsoft Teams problemer med Exchange Server interaktion.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
