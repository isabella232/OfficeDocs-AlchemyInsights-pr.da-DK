---
title: Kryptere bestemte mails automatisk fra Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524015"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Kryptere bestemte mails automatisk fra Office 365

1. I [Exchange Administration skal du](https://outlook.office365.com/ecp/)vælge **mailflow > regler.** 
2. Klik på **ikonet Nyt (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**
3. Skriv **et** navn til reglen under Navn, f.eks. *Kryptér alle meddelelser.*
4. Vælg **[Anvend på alle** meddelelser] i Anvend denne **regel, hvis.** 
5. Klik på **Vælg et ud** for feltet Gør **følgende.** 
6. Vælg **Kryptér i rullemenuen RMS-skabelon,** og klik derefter på **OK.** (Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering. Men du kan tilføje den!)
7. Markér **afkrydsningsfeltet Overhold denne regel med alvorsniveau,** og vælg derefter det ønskede niveau. Hvis din virksomhed har kontraktmæssige forpligtelser til at sende alle mails krypteret, anbefaler jeg, at niveauet angives til **Høj.**
8. Klik **på Gennemtving under Vælg en model** til denne **regel.** 
9. Vælg eventuelt valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).
10. Klik på **Gem**.

> [!IMPORTANT]
> Du kan altid vende tilbage og redigere denne regel senere.

Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

