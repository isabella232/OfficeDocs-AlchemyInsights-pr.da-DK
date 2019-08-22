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
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539095"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificere når eksterne e-mail-videresendelse er konfigureret til postkasser

Når en bruger i Office 365 konfigurerer eksterne e-mail-videresendelse på en postkasse, overvåges aktiviteten, som en del af **Set-Mailbox** -cmdlet. Du kan se aktiviteten ved hjælp af overvågning log Søg i Security & Overholdelsescenter.

1. Log på [Office 365 sikkerhed & Overholdelsescenter](https://protection.office.com/).

2. Gå til **Søg** > **revision log** søgeside.

3. Vælg datointervallet i felterne **startdato** og **slutdato** . Du behøver ikke at angive et brugernavn. Kontroller feltet **aktiviteter** er indstillet til at **få vist resultater for alle aktiviteter**.

4. Klik på **Søg**.

Klik på **Filtrerede resultater** i resultaterne, og skriv **Sæt postkasse** i filterboksen aktivitet. Vælg en revisionspost i resultaterne. **Oplysninger om** mærke, klik på **flere oplysninger**. Du skulle se på detaljerne for hver revisionspost til at bestemme, om aktiviteten vedrører e-mail videresendelse.

- **ObjectId**: alias værdien af den postkasse, der er blevet ændret.

- **Parametre**: _ForwardingSmtpAddress_ angiver e-mail-adressen til destinationen.

- **Bruger-id**: den bruger, der konfigureret e-mail-videresendelse på postkassen i feltet **ObjectId** .

Yderligere oplysninger finder du [fastlægge, der har konfigureret e-mail videresendes til en postkasse](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
