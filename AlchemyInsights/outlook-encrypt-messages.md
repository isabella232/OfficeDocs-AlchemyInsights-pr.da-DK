---
title: S/MIME i Outlook på internettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764866"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptere mails i Outlook

Microsoft 365-meddelelseskryptering er baseret på Azure RMS (Microsoft Azure Rights Management), som er en del af Azure Information Protection. Hvis dit abonnement omfatter Azure Rights Management eller Azure Information Protection, **behøver du ikke at foretage dig noget for manuelt at aktivere eller aktivere** Rights Management Service.

Baseret på kundefeedback vil vi ikke længere gøre det muligt for Exchange mailflowregler automatisk at kryptere udgående e-mails, der indeholder bestemte typer følsomme oplysninger i din lejer som standard. I stedet giver vi detaljerede instruktioner om, hvordan I selv kan gøre det. Yderligere oplysninger om, hvordan du opretter en transportregel til kryptering af følsomme oplysninger, finder du i [denne artikel](https://aka.ms/OmeEtr).

- Hvis du bruger Outlook på internettet (tidligere **OWA**): Når du skriver en mail, skal du blot klikke på **Beskyt** i OWA. Dette gælder tilladelsen "Videresend ikke". Klik på **Skift tilladelse,** og vælg **Krypter** for kun at kryptere meddelelsen.

- Hvis du bruger **Outlook-klient**: Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge **Tilladelser til** > **indstillinger**og derefter vælge den beskyttelsesindstilling, du har brug for.

- Hvis du automatisk vil **kryptere alle mails,** der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en regel for transport af mailflow i Exchange Administration. Detaljerede instruktioner findes i [denne supportartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

