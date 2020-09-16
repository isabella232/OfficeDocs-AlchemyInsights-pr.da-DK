---
title: S/MIME i Outlook på internettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772256"
---
# <a name="encrypt-email-messages-in-outlook"></a>Krypter mails i Outlook

Microsoft 365-meddelelseskryptering er baseret på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure information Protection. Hvis dit abonnement omfatter Azure Rights Management eller Azure information Protection, behøver **du ikke at foretage nogen handlinger for at aktivere eller aktivere** tjenesten Rights Management manuelt.

Baseret på kundefeedback kan vi ikke længere aktivere regler for Exchange-mail flow for automatisk at kryptere udgående mails, der indeholder bestemte typer følsomme oplysninger i din lejer som standard. I stedet giver vi detaljerede anvisninger til, hvordan du kan gøre det selv. Du kan finde flere oplysninger om, hvordan du opretter en transportregel for at kryptere følsomme oplysninger, i [denne artikel](https://aka.ms/OmeEtr).

- Hvis du bruger Outlook på internettet (tidligere **OWA**): når du skriver en mail, skal du blot klikke på **Beskyt** i OWA. Dette vil anvende tilladelsen "Videresend ikke". Klik på **Rediger tilladelse** , og vælg **Krypter** for kun at kryptere meddelelsen.

- Hvis du bruger **Outlook-klient**: Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge **Indstillinger for**  >  **tilladelser**og derefter vælge den beskyttelses indstilling, du har brug for.

- Hvis du **automatisk vil kryptere alle mails** , der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en transportregel for forsendelses strømmen i Exchange Admin Center. Der findes detaljerede instruktioner i [denne supportartikel](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

