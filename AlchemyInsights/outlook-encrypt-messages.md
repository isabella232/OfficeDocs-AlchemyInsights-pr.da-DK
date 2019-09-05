---
title: S/MIME i Outlook på internettet
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752854"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptér e-mail-meddelelser i Outlook

Office 365-meddelelseskryptering er baseret på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure information Protection. Hvis dit abonnement omfatter Azure Rights Management eller Azure information Protection, **behøver du ikke foretage dig noget for manuelt at aktivere eller aktivere** Rights Management-tjenesten.

Baseret på kundefeedback vil vi ikke længere aktivere Exchange mail flow-regler for automatisk at kryptere udgående mails, der indeholder visse typer af følsomme oplysninger i din lejer som standard. I stedet giver vi detaljerede instruktioner om, hvordan du kan gøre det selv. Yderligere oplysninger om, hvordan du opretter en transportregel til kryptering af følsomme oplysninger, finder du i [denne artikel](https://aka.ms/OmeEtr).

- Hvis du bruger Outlook på internettet (tidligere **OWA**): når du komponerer en e-mail-besked, skal du blot klikke på **Beskyt** i OWA. Dette vil gælde "Videresend ikke"-tilladelse. Klik på **Skift tilladelse** , og vælg **Kryptér** for kun at kryptere meddelelsen.

- Hvis du **bruger Outlook-klient**: Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge **Options** > **tilladelser**og derefter vælge den ønskede beskyttelses indstilling.

- Hvis du **automatisk vil kryptere alle mails** , der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en transportregel for e-mail-strømmen i Exchange administration. Detaljerede anvisninger er angivet i [denne supportartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

