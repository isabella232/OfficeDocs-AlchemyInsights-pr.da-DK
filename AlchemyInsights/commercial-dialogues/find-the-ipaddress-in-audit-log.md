---
title: Find IP-adressen i overvågningsloggen
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902254"
---
# <a name="find-the-ip-address-in-audit-log"></a>Find IP-adressen i overvågningsloggen

Den IP-adresse, der svarer til en aktivitet, der er udført af en bruger eller administrator, vises i overvågningslogfilerne. Klientoplysningerne logføres også. Sådan identificerer du IP-adressen:

1. Gør en af følgende handlinger:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til **Løsningsrevision** \> . Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I portalen Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Hvis du ser en meddelelse om, at du skal aktivere overvågning, skal du bare aktivere det nu. Hvis denne funktion ikke er aktiveret, vil søgeresultaterne ikke kunne trække data fra tidligere datoer.

2. Kontrollér, **at** fanen Søg er markeret **på siden** Overvågning, og konfigurer derefter følgende indstillinger:
   - **Dato- og tidsinterval:** Markér dato/klokkeslæt-området i **felterne Start** **og** Slut.
   - **Aktiviteter:** Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på listen. Ellers returneres **standardværdien Vis resultater for** alle aktiviteter. Bemærk, at visse aktiviteter muligvis ikke er tilgængelige for markering. Disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er markeret.
   - **Brugere:** Acceptér den tomme standardværdi for at returnere resultater for alle brugere, eller angiv en eller flere brugere.

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.**

4. I resultaterne skal du klikke **på Filtrer resultater** og **skrive Angiv postkasse** i feltet Aktivitetsfilter.

5. Vælg en overvågningspost i resultaterne for at åbne pop **op-dialogboksen** Detaljer.

Få mere at vide under [Søg i overvågningsloggen for at undersøge almindelige supportproblemer.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
