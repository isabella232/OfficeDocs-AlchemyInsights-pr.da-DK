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
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899878"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificer, hvornår ekstern videresendelse af mail er konfigureret i postkasser

Når en Microsoft 365 konfigurerer ekstern videresendelse af mail i en postkasse, overvåges aktiviteten som en del af **Set-Mailbox** cmdlet'en. Du kan se aktiviteten ved hjælp af søgning i overvågningsloggen. Sådan gør du det.

1. Gør et af følgende:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til **Løsningsrevision** \> . Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I portalen Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://sip.security.microsoft.com/auditlogsearch> .

2. Kontrollér, **at** fanen Søg er markeret **på siden** Overvågning, og konfigurer derefter følgende indstillinger:
   - Vælg området for dato/klokkeslæt i **felterne Start** **og** Slut.
   - Kontrollér, **at feltet** Aktiviteter indeholder Vis resultater for alle **aktiviteter.**

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.**

4. I resultaterne skal du klikke **på Filtrer resultater** og **skrive Angiv postkasse** i feltet Aktivitetsfilter.

5. Vælg en overvågningspost i resultaterne. Klik på **Flere** oplysninger i pop **op-menuen Detaljer.** Du skal se på detaljerne for hver overvågningspost for at afgøre, om aktiviteten er relateret til videresendelse af mail.

   - **Objekt-id:** Aliasværdien for den postkasse, der blev ændret.
   - **Parametre:** _ForwardingSmtpAddress_ angiver målmailadressen.
   - **UserId:** Den bruger, der konfigurerede videresendelse af mail i postkassen i **feltet ObjectId.**

Du kan få mere at vide [under Fastslå, hvem der har konfigureret videresendelse af mail for en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
