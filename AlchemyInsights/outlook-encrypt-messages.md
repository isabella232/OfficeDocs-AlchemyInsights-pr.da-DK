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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010718"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptér mails i Outlook

Microsoft 365 Meddelelseskryptering er bygget på Microsoft Azure Rights Management (Azure RMS), som er en del af Azure Information Protection. Hvis dit abonnement omfatter Azure Rights Management eller Azure Information Protection, behøver du ikke at udføre nogen handlinger for at aktivere eller **aktivere** Rights Management Service manuelt.

Baseret på kundefeedback aktiverer vi ikke længere regler Exchange for mailflow automatisk at kryptere udgående mails, der indeholder bestemte typer af følsomme oplysninger i din lejer som standard. I stedet giver vi dig detaljerede instruktioner om, hvordan du kan gøre det selv. Du kan finde flere oplysninger om, hvordan du opretter en transportregel for at kryptere følsomme oplysninger, [i denne artikel.](https://aka.ms/OmeEtr)

- Hvis du Outlook på internettet (tidligere **OWA**): Når du skriver en mail, skal du blot klikke på **Beskyt** i OWA. Dette vil anvende tilladelsen "Videressendelse ikke". Klik **på Rediger tilladelse,** og vælg **Kryptér** for kun at kryptere meddelelsen.

- Hvis du **bruger Outlook-klienten:** Hvis du vil sende en krypteret meddelelse fra Outlook 2013 eller 2016 eller Outlook 2016 til Mac, skal du vælge Indstillinger Tilladelser og derefter vælge den beskyttelsesindstilling, du skal  >  bruge.

- Hvis **du automatisk vil kryptere** alle de mails, der sendes til bestemte modtagere eller eksterne partnerorganisationer, skal du oprette en mailflow-transportregel i Exchange Administration. Detaljerede instruktioner findes i [denne supportartikel.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

