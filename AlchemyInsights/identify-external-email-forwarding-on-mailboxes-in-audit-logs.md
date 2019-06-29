---
title: Identificere eksterne e-mail-videresendelse på postkasser i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383091"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificere når eksterne e-mail-videresendelse er konfigureret til postkasser

Når brugeren konfigurerer eksterne e-mail-videresendelse på en postkasse, overvåges aktiviteten, som en del af **Set-Mailbox** -cmdlet. Du kan se aktiviteten ved hjælp af overvågning log Søg i Security & Overholdelsescenter.

1. Log på [Office 365 & overholdelse Sikkerhedscenter](https://protection.office.com/)

2. Klik på **Søg og undersøgelse** , og vælg **Revision Log søgning**.

3. Vælg datointervallet i felterne **startdato** og **slutdato** . Du behøver ikke at angive et brugernavn. Kontroller feltet **aktiviteter** er indstillet til at **få vist resultater for alle aktiviteter**.

4. Klik på **Søg**.

Klik på **Filtrerede resultater** i resultaterne, og skriv **Sæt postkasse** i filterboksen aktivitet. Vælg en revisionspost i resultaterne. **Oplysninger om** mærke, klik på **flere oplysninger**. Du skulle se på detaljerne for hver revisionspost til at bestemme, om aktiviteten vedrører e-mail videresendelse.

- **ObjectId**: alias værdien af den postkasse, der er blevet ændret.

- **Parametre**: _ForwardingSmtpAddress_ angiver e-mail-adressen til destinationen.

- **Bruger-id**: den bruger, der konfigureret e-mail-videresendelse på postkassen i feltet **ObjectId** .

Yderligere oplysninger finder du [fastlægge, der har konfigureret e-mail videresendes til en postkasse](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
