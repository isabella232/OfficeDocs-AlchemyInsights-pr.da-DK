---
title: Kryptere Office 365-mails, der sendes til bestemte domæner, automatisk
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524003"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Kryptere Office 365-mails, der sendes til bestemte domæner, automatisk

1. I [Exchange Administration skal du](https://outlook.office365.com/ecp/)vælge **mailflow > regler.** 
2. Klik på **ikonet Nyt (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**
3. Skriv **et navn** til reglen under Navn, f.eks. Kryptér *meddelelser, der sendes contoso.com.*
4. I **Anvend denne regel, hvis,** skal **du vælge > domænet er.** 
5. Angiv navnet på domænet, f.eks. **contoso.com.**
6. Klik på **ikonet Tilføj (+),** og klik derefter på **OK.**
7. Klik på **Vælg et ud** for feltet Gør **følgende.** 
8. Vælg **Kryptér i rullemenuen RMS-skabelon,** og klik derefter på **OK.** (Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering. Men du kan tilføje den!)
9. Vælg eventuelt valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).
10. Klik på **Gem**.

> [!IMPORTANT]
> Du kan altid vende tilbage og redigere denne regel senere.

Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)