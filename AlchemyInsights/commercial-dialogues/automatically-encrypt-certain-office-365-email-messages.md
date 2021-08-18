---
title: Automatisk kryptere bestemte Office 365 e-mail-meddelelser
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
ms.openlocfilehash: b15a72ced4921b3df1b7105837592781188a2a25
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327968"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatisk kryptere bestemte Office 365 e-mail-meddelelser

Du kan automatisk kryptere meddelelser, som brugere sender til bestemte eksterne personer eller organisationer. Det gør du ved at udføre følgende trin:

1. Vælg [Exchange regler fra](https://outlook.office365.com/ecp/)Administration **for mailflow > regler.** 
2. Klik på **ikonet Ny (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**
3. Under **Navn** skal du skrive et navn til reglen, f.eks. *Kryptér meddelelser, der sendes DrToniRamos@gmail.com*.
4. I **Anvend denne regel hvis** skal du vælge Modtageren skal > denne **person.** 
5. I vinduet **Vælg medlemmer** skal du vælge navnet på den person, krypteringsreglen skal gælde for, og derefter skal du klikke på **Tilføj.** 
6. Når du er færdig med at tilføje brugere, skal du klikke **på OK.**
7. Ud for feltet **Gør følgende skal** du klikke på Vælg **en**. 
8. I **rullemenuen RMS-skabelon** skal du vælge **Kryptér** og derefter klikke på **OK**. Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering. Men du kan tilføje den!)
9. Vælg et valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for overskuelighed).
10. Klik på **Gem**.

**Vigtigt!** Du kan altid vende tilbage og redigere denne regel senere.

Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

