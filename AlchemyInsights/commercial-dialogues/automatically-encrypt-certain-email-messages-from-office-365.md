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
ms.openlocfilehash: e050074f26025906561237c9ef487ed4743f93b1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322243"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Kryptere bestemte mails automatisk fra Office 365

1. Vælg [Exchange regler for](https://outlook.office365.com/ecp/) **mailflow i Administration > regler.** 
2. Klik på **ikonet Ny (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**
3. Skriv **et** navn til reglen under Navn, f.eks. *Kryptér alle meddelelser*.
4. I **Anvend denne regel hvis** skal du vælge **[Anvend på alle meddelelser]**. 
5. Ud for feltet **Gør følgende skal** du klikke på Vælg **en**. 
6. I **rullemenuen RMS-skabelon** skal du vælge **Kryptér** og derefter klikke på **OK**. Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering. Men du kan tilføje den!)
7. Markér **afkrydsningsfeltet Overhold denne regel med alvorsniveau,** og vælg derefter det ønskede niveau. Hvis din virksomhed har kontraktmæssige forpligtelser til at sende alle mails krypteret, anbefaler jeg, at niveauet angives til **Høj.**
8. Klik **på Gennemtving under Vælg en model** for denne **regel.** 
9. Vælg et valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for overskuelighed).
10. Klik på **Gem**.

**Vigtigt!** Du kan altid vende tilbage og redigere denne regel senere.

Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

