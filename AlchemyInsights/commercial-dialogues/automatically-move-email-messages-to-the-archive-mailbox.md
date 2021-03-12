---
title: Flyt automatisk mails til arkivpostkassen
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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744546"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Flyt automatisk mails til arkivpostkassen

Sådan konfigurerer du en politik til automatisk at flytte en brugers gamle mail til arkivpostkassen:

1. Gå til [**Security & Arkiv for**](https://go.microsoft.com/fwlink/p/?linkid=2077143)styring af overholdelse af  >  **data**  >  **for** at bekræfte, at en arkivpostkasse er aktiveret for brugeren. Hvis den ikke er blevet vist, skal du **klikke på** **Aktivér og** derefter på Ja i advarselsfeltet.
2. Gå til [**Exchange Administration for at > overholdelsesstyring > opbevaringsmærker.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Vælg ikonet + og vælg derefter **automatisk at anvende på hele postkassen.**
4. Tildel et navn til opbevaringsmærket, og vælg **Flyt til arkiv.** For opbevaringsperioden skal du angive den ønskede tid, f.eks. 90 dage. Klik på **Gem**.
5. Opret nu en opbevaringspolitik: Vælg **opbevaringspolitikker,** vælg ikonet for at tilføje en ny politik.
6. Tildel et navn til opbevaringspolitikken, klik og rul derefter for at finde og tilføje det opbevaringsmærke, du lige har oprettet. Klik på **Gem**.
7. Til sidst skal du anvende opbevaringspolitikken på brugerens postkasse: Stadig i Exchange Administration skal du gå til **modtagernes**  >  **postkasser.** Vælg alle de brugere, du vil anvende politikken på, og vælg derefter **Rediger** (blyantsikonet).
8. Klik på postkassefunktioner **i dialogboksen.** Anvend **den politik,** du lige har oprettet, under Opbevaringspolitik > **Gem.**
9. Hvis du vil have vejledning i at anvende politikken på alle brugere, skal [du se Anvend en opbevaringspolitik på postkasser.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
