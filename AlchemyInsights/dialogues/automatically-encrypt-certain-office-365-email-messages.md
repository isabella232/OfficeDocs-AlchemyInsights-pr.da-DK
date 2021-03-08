---
title: Kryptere visse Office 365-mails automatisk
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524011"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Kryptere visse Office 365-mails automatisk

Du kan automatisk kryptere meddelelser, som brugere sender til bestemte eksterne personer eller organisationer. Det gør du ved at udføre følgende trin:

1. I [Exchange Administration skal du](https://outlook.office365.com/ecp/)vælge **mailflow > regler.** 
2. Klik på **ikonet Nyt (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**
3. Skriv **et navn** til reglen under Navn, f.eks. Kryptér *meddelelser, der sendes til DrToniRamos@gmail.com.*
4. I **Anvend denne regel, hvis** skal du vælge > er denne **person.** 
5. Vælg navnet **på den** person, du vil anvende krypteringsreglen på, i vinduet Vælg medlemmer, og klik derefter på **Tilføj.** 
6. Klik på OK, når du er færdig med at tilføje **brugere.**
7. Klik på **Vælg et ud** for feltet Gør **følgende.** 
8. Vælg **Kryptér i rullemenuen RMS-skabelon,** og klik derefter på **OK.** (Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering. Men du kan tilføje den!)
9. Vælg eventuelt valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).
10. Klik på **Gem**.

> [!IMPORTANT]
> Du kan altid vende tilbage og redigere denne regel senere.

Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

