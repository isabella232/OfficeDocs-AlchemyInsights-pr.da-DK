---
title: Krypter automatisk Office 365 mails, der sendes til visse domæner
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082180"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Krypter automatisk Office 365 mails, der sendes til visse domæner

1. Vælg [mailflow Exchange regler](https://outlook.office365.com/ecp/) **fra > Administration .** 
2. Klik på **ikonet Ny (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**
3. Under **Navn** skal du angive et navn til reglen, f.eks. *Kryptér meddelelser, der sendes contoso.com*.
4. I **Anvend denne regel hvis** skal du vælge Modtageren > domæne **er**. 
5. Angiv navnet på domænet, f.eks. **contoso.com**.
6. Klik på **ikonet Tilføj (+),** og klik derefter på **OK.**
7. Ud for feltet **Gør følgende skal** du klikke på Vælg **en**. 
8. I **rullemenuen RMS-skabelon** skal du vælge **Kryptér** og derefter klikke på **OK**. Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering. Men du kan tilføje den!)
9. Vælg et valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).
10. Klik på **Gem**.

> [!IMPORTANT]
> Du kan altid vende tilbage og redigere denne regel senere.

Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)