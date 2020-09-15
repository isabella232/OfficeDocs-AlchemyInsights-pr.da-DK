---
title: Identificer ekstern videresendelse af mail i postkasser i overvågningslogge
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696291"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificer, hvornår videresendelse af ekstern mail er konfigureret på postkasser

Når en Microsoft 365-bruger konfigurerer ekstern videresendelse af mail i en postkasse, overvåges aktiviteten som en del af cmdlet'en **set-Mailbox** . Du kan se aktiviteten ved hjælp af søgning i overvågningsloggen i sikkerheds & overholdelses Center.

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til søgesiden **Søg i**  >  **overvågningslogfil** .

3. Vælg datointervallet i felterne **Start dato** og **Slutdato** . Du behøver ikke at angive et Brugernavn. Kontrollér, at feltet **aktiviteter** er indstillet til at **vise resultater for alle aktiviteter**.

4. Klik på **Søg**.

I resultaterne skal du klikke på **filter resultater** og skrive **set-postkasse** i feltet aktivitets filter. Vælg en revisionspost i resultaterne. Klik på **flere oplysninger**i pop op-vinduet **detaljer** . Du skal se nærmere på detaljerne for hver revisionspost for at afgøre, om aktiviteten er relateret til videresendelse af mail.

- **ObjectId**: alias værdien for den postkasse, der blev ændret.

- **Parametre**: _ForwardingSmtpAddress_ Angiver destinations mailadressen.

- **UserID**: den bruger, der har konfigureret videresendelse af mails, i feltet ObjectId i feltet **ObjectId** .

Hvis du vil have mere at vide, skal du se [bestemme, hvem der skal konfigurere videresendelse af mail for en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
