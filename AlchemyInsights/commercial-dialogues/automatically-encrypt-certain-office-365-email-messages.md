---
title: Kryptere bestemte Office 365 automatisk
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
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949561"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Kryptere bestemte Office 365 automatisk

Du kan automatisk kryptere meddelelser, som brugere sender til bestemte eksterne personer eller organisationer. Det gør du ved at udføre følgende trin:

1. Vælg [mailflow Exchange regler](https://outlook.office365.com/ecp/) **fra > Administration .** 
2. Klik på **ikonet Ny (+),** og klik derefter på **Anvend Office 365-meddelelseskryptering og rettighedsbeskyttelse på meddelelser.**
3. Under **Navn** skal du angive et navn til reglen, f.eks. *Kryptér meddelelser, der sendes DrToniRamos@gmail.com*.
4. I **Anvend denne regel hvis** skal du vælge **Modtagerens > er denne person**. 
5. I vinduet **Vælg medlemmer** skal du vælge navnet på den person, krypteringsreglen skal gælde for, og derefter skal du klikke på **Tilføj.** 
6. Når du er færdig med at tilføje brugere, skal du klikke **på OK.**
7. Ud for feltet **Gør følgende skal** du klikke på Vælg **en**. 
8. I **rullemenuen RMS-skabelon** skal du vælge **Kryptér** og derefter klikke på **OK**. Hvis du ikke kan se denne indstilling, betyder det, at din plan ikke omfatter automatisk kryptering. Men du kan tilføje den!)
9. Vælg et valgfrit valg (på en liste over valgfrie valg, du kan foretage på nuværende tidspunkt, hvoraf mange kan stå med standardindstillingen for enkelhed).
10. Klik på **Gem**.

> [!IMPORTANT]
> Du kan altid vende tilbage og redigere denne regel senere.

Du kan finde flere oplysninger om oprettelse af regler for kryptering i [Definere regler for mailflow for at kryptere mails i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

