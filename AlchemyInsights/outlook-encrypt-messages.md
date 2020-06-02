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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511502"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptere mails i Outlook

Microsoft 365 Message Encryption er baseret på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure Information Protection. Hvis dit abonnement omfatter Azure Rights Management eller Azure Information Protection, **behøver du ikke at foretage dig noget for manuelt at aktivere eller aktivere** Tjenesten Rights Management.

Baseret på kundefeedback vil vi ikke længere gøre det muligt for Exchange-mailflowregler automatisk at kryptere udgående mails, der indeholder bestemte typer følsomme oplysninger i din lejer som standard. I stedet giver vi detaljerede instruktioner om, hvordan I selv kan gøre det. Yderligere oplysninger om, hvordan du opretter en transportregel til kryptering af følsomme oplysninger, finder du i [denne artikel](https://aka.ms/OmeEtr).

- Hvis du bruger Outlook på internettet (tidligere **OWA):** Når du skriver en mail, skal du blot klikke på **Beskyt** i OWA. Dette gælder tilladelsen "Videresend ikke". Klik på **Skift tilladelse,** og vælg **Krypter** for kun at kryptere meddelelsen.

- Hvis du vil bruge **Outlook-klient**: Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge **Indstillinger**tilladelser og derefter vælge den  >  **beskyttelsesindstilling,** du har brug for.

- Hvis du automatisk vil **kryptere alle mails,** der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en regel for mailflowtransport i Exchange Administration. Der findes detaljerede instruktioner i [denne supportartikel](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

