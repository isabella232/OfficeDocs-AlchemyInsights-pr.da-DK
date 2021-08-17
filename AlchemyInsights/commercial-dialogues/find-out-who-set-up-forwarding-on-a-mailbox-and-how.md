---
title: Find ud af, hvem der har konfigureret videresendelse på en postkasse, og hvordan
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895173"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Find ud af, hvem der har konfigureret videresendelse på en postkasse, og hvordan

Hvis ekstern videresendelse blev indstillet på en postkasse, overvåges aktiviteten som en del af **cmdlet'en Set-Mailbox.** Sådan finder du aktiviteten i overvågningsloggen:

1. Gør en af følgende handlinger:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til **Løsningsrevision** \> . Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://security.microsoft.com/auditlogsearch> .

   > [!NOTE]
   > Hvis du ser en meddelelse om, at du skal aktivere overvågning, skal du bare aktivere det nu. Hvis denne funktion ikke er aktiveret, kan søgeresultaterne ikke trække data fra tidligere datoer.

2. Kontrollér, **at** fanen Søg er markeret **på siden** Overvågning, og konfigurer derefter følgende indstillinger:
   - Vælg området for dato/klokkeslæt i **felterne Start** **og** Slut.
   - Kontrollér, **at feltet** Aktiviteter indeholder Vis resultater for alle **aktiviteter.**

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.**

4. Klik på kolonnen Aktivitet i **resultaterne** for at sortere resultaterne, og se efter **Angiv postkasseposter.**

5. Vælg en aktivitet i resultaterne for at åbne pop op-dialogboksen med detaljer. Du skal se på detaljerne for hver overvågningspost for at afgøre, om aktiviteten er relateret til videresendelse af mail:
   - **Objekt-id:** Aliasværdien for den postkasse, der blev ændret.
   - **Parametre:** _ForwardingSmtpAddress_ angiver målmailadressen.
   - **UserId:** Den bruger, der konfigurerede videresendelse af mail i postkassen i **feltet ObjectId.**

Du kan få mere at vide [under Fastslå, hvem der har konfigureret videresendelse af mail for en postkasse](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
