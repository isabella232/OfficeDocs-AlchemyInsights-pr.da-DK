---
title: Identificer ekstern videresendelse af mail i postkasser i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630243"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificer, hvornår ekstern videresendelse af mail er konfigureret i postkasser

Når en Microsoft 365 konfigurerer ekstern videresendelse af mail i en postkasse, overvåges aktiviteten som en del af **Set-Mailbox-cmdlet'en.** Du kan se aktiviteten ved hjælp af søgning i overvågningsloggen i & Security & Compliance Center.

1. Log på Microsoft 365 [Compliance Center.](https://protection.office.com/)

2. Gå til **søgesiden**  >  **for søgeloggen i overvågningsloggen.**

3. Vælg datointervallet i **felterne Startdato** **og** Slutdato. Du behøver ikke at angive et brugernavn. **Bekræft, at** feltet Aktiviteter er **indstillet til Vis resultater for alle aktiviteter.**

4. Klik **på Søg**.

I resultaterne skal du klikke **på Filtrer resultater** og **skrive Angiv postkasse** i feltet Aktivitetsfilter. Vælg en overvågningspost i resultaterne. Klik på **Flere** oplysninger i pop **op-menuen Detaljer.** Du skal se på detaljerne for hver overvågningspost for at afgøre, om aktiviteten er relateret til videresendelse af mail.

- **Objekt-id:** Aliasværdien for den postkasse, der blev ændret.

- **Parametre:** _ForwardingSmtpAddress_ angiver målmailadressen.

- **UserId:** Den bruger, der konfigurerede videresendelse af mail i postkassen i **feltet ObjectId.**

Du kan få mere at vide [under Fastslå, hvem der har konfigureret videresendelse af mail for en postkasse](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
