---
title: Identificer ekstern videresendelse af mail i postkasser i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508946"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificer, hvornår ekstern videresendelse af mail er konfigureret i postkasser

Når en Microsoft 365-bruger konfigurerer ekstern videresendelse af mail i en postkasse, overvåges aktiviteten som en del af **cmdlet'en set-postkasse.** Du kan se aktiviteten ved hjælp af søgning i overvågningsloggen i Sikkerheds- & Compliance Center.

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til søgesiden for søgesøgning i søgeloggen søge i søgeloggen **for søgeloggen søge**i søgeloggen for  >  **søgesøgning.**

3. Vælg datointervallet i felterne **Startdato** og **Slutdato.** Du behøver ikke at angive et brugernavn. Kontroller, at feltet **Aktiviteter** er angivet til **Vis resultater for alle aktiviteter**.

4. Klik på **Søg**.

Klik på **Filtrer resultater** i resultaterne, og skriv **Angiv postkasse** i aktivitetsfilterfeltet. Vælg en overvågningspost i resultaterne. Klik på **Flere oplysninger**i pop op-vinduet **Detaljer** . Du skal se på detaljerne i hver overvågningspost for at afgøre, om aktiviteten er relateret til videresendelse af e-mail.

- **ObjectId**: Aliasværdien for den postkasse, der blev ændret.

- **Parametre**: _ForwardingSmtpAddress_ angiver destinations-e-mailadressen.

- **UserId**: Den bruger, der har konfigureret videresendelse af mail på postkassen i feltet **ObjectId.**

Du kan finde flere oplysninger [under Bestemme, hvem der konfigurerer videresendelse af mail til en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
