---
title: 726 Blokering af videresendelse af mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059626"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokere eller fjerne blokeringen af videresendelse af mail

Hvis du vil aktivere eller deaktivere videresendelse af mail for en bestemt postkasse, skal du [se Konfigurer videresendelse af mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

På lejerniveau udføres styringen af ekstern videresendelse ved hjælp af politikken for udgående spam. Du kan kontrollere politikken for udgående spamfilter fra Security and Compliance [Center](https://protection.office.com/antispam) her eller ved hjælp af kommandoen [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Hvis du får følgende fejlmeddelelse: **"550 5.7.520 Access denied, Your organization does not allow external forwarding",** sørg for, at politikken er konfigureret til at aktivere Ekstern automatisk videresendelse.

**Bemærk!** Det anbefales, at du holder Ekstern autoforward deaktiveret på din standard politik for udgående spamfilter og kun aktiverer den for de brugere, der har brug for ekstern videresendelse, ved at oprette en brugerdefineret politik for disse brugere. Du kan læse mere i [Konfiguration af ekstern videresendelse af mail i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).