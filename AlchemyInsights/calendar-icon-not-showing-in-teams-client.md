---
title: Kalenderikonet vises ikke i Teams-klient
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989585"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalenderikonet vises ikke i Teams-klient

Fanen Kalender i Teams kræver adgang til en Exchange-postkasse via Exchange Webtjenester. Exchange-postkassen kan være online eller lokal. Onlinebrugere, der ikke kan se fanen Kalender, skal sørge for, at de [har licens til en Exchange Online-postkasse, og at postkassen er aktiveret](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Hvis brugeren har en gyldig postkasse i Exchange Online, men stadig ikke kan se fanen Kalender, er der måske problemer med netværket. Brug [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/), og kør **forbindelsestesten for Microsoft Exchange-webtjenester** for den berørte bruger.

Læs til sidst [Teams-apps – politikker om konfiguration af apps](https://admin.teams.microsoft.com/policies/app-setup) for at sikre, at appen Kalender ikke er fjernet fra den politik, der gælder for brugeren (sandsynligvis **Global (standard for hele organisation standard)**.

Hvis dine brugere arbejder lokalt, skal du bekræfte, at din hybridkonfiguration er i orden. Brug [Guiden Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) til fejlfinding.

Bemærk, at [Teams kræver Exchange 2016 CU3 eller højere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
