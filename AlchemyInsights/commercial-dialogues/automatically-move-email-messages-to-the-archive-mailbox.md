---
title: Automatisk flytte mails til arkivpostkassen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059220"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatisk flytte mails til arkivpostkassen

Sådan konfigurerer du en politik til automatisk at flytte en brugers gamle mail til arkivpostkassen:

1. Gå til [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data  >  **Governance**  >  **Archive** for at bekræfte, at en arkivpostkasse er aktiveret for brugeren. Hvis det ikke er, skal du klikke **på Aktivér** **og derefter** Ja i advarselsfeltet.
2. Gå til [**Exchange Administration > overholdelsesstyring > opbevaringsmærker.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Vælg +-ikonet, og vælg **derefter automatisk anvend på hele postkassen**.
4. Tildel et navn til opbevaringsmærket, og vælg **Flyt til arkiv**. For opbevaringsperioden skal du angive den ønskede tid, f.eks. 90 dage. Klik på **Gem**.
5. Opret nu en opbevaringspolitik: Vælg **opbevaringspolitikker**, vælg ikonet for at tilføje en ny politik.
6. Tildel opbevaringspolitikken et navn, klik og rul derefter for at finde og tilføje det opbevaringsmærke, du lige har oprettet. Klik på **Gem**.
7. Til sidst skal du anvende opbevaringspolitikken på brugerens postkasse: stadig i Exchange Administration skal du gå **til modtagernes**  >  **postkasser.** Vælg alle de brugere, du vil anvende politikken på, og vælg derefter **Rediger** (blyantsikonet).
8. I dialogboksen skal du klikke på **Postkassefunktioner**. Under **Opbevaringspolitik skal** du anvende den politik, du lige har oprettet > **Gem.**
9. Hvis du vil have vejledning i at anvende politikken på alle brugere, [skal du se Anvend en opbevaringspolitik på postkasser.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
