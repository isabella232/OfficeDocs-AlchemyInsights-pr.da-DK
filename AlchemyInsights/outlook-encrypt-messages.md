---
title: S/MIME-i Outlook på internettet
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666834"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptere e-mails i Outlook

Office 365 meddelelseskryptering er bygget på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure beskyttelse af oplysninger. Hvis abonnementet omfatter Azure Rights Management eller Azure beskyttelse af oplysninger, **du behøver ikke at udføre handlinger manuelt aktivere eller aktivere** Rights Management-tjenesten.

Baseret på kundefeedback, vil vi ikke længere aktivere Exchange flow postregler kryptere udgående e-mail, der indeholder visse typer følsomme oplysninger i din lejer som standard automatisk. I stedet vores detaljerede instruktioner om, hvordan du kan gøre det vigtige. Du kan finde yderligere oplysninger om, hvordan du opretter en regel, transport for at kryptere følsomme oplysninger [i denne artikel](https://aka.ms/OmeEtr).

- Hvis du bruger Outlook på internettet (tidligere **OWA**): Når du skriver en e-mail, skal du klikke på **Beskyt** i OWA. Dette gælder "Do ikke fremad" tilladelse. Klik på **Skift tilladelse** og vælge **Krypter** kun kryptere meddelelsen.

- Hvis du bruger **Outlook-klienten**: Vælg **Indstillinger**for at sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller 2016 Outlook til Mac, > **tilladelser**og derefter vælge indstillingen beskyttelse du har brug for.

- Til **automatisk at kryptere alle e-mails** sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en regel for transport flow i Exchange Admin Center. Der findes detaljerede anvisninger i [denne supportartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

