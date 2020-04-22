---
title: Identificere ekstern videresendelse af mail på postkasser i overvågningslogfiler
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
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716454"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificer, hvornår ekstern videresendelse af mail er konfigureret i postkasser

Når en Microsoft 365-bruger konfigurerer ekstern videresendelse af mail på en postkasse, overvåges aktiviteten som en del af **cmdlet'en Set-Mailbox.** Du kan se aktiviteten ved hjælp af overvågningslogsøgning i Sikkerheds& Compliance Center.

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til**søgesiden for søgefilen til søgeovervågning** i **søgefilen** > til søgning i søgeområdet.

3. Vælg datointervallet i felterne **Startdato** **og Slutdato.** Du behøver ikke at angive et brugernavn. Kontroller, at feltet **Aktiviteter** er angivet til Vis resultater for **alle aktiviteter**.

4. Klik på **Søg**.

Klik på **Filtrer resultater** i resultaterne, og skriv **Set-Postkasse** i feltet aktivitetsfilter. Vælg en overvågningspost i resultaterne. Klik på Flere oplysninger i pop **op-vinduet** **Detaljer** . Du skal se på detaljerne for hver overvågningspost for at afgøre, om aktiviteten er relateret til videresendelse af e-mail.

- **ObjectId**: Aliasværdien for den postkasse, der blev ændret.

- **Parametre**: _Videresendelse SmtpAddress_ angiver destinationsmailadressen.

- **UserId**: Den bruger, der konfigurerede videresendelse af mail på postkassen i **feltet ObjectId.**

Du kan finde flere oplysninger [under Bestemme, hvem der konfigurerer videresendelse af mail for en postkasse](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
