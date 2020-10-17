---
title: 726 blokere mail videresendelse
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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473095"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokere eller fjerne blokeringen af videresendelse af mail

Hvis du vil aktivere eller deaktivere videresendelse af mail for en bestemt postkasse, skal du se [konfigurere videresendelse af mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

På lejerniveau er kontrol af ekstern videresendelse udført ved hjælp af den udgående spam politik. Du kan kontrollere politikken for udgående spamfilter fra sikkerhed og overholdelses Center [her] ( https://protection.office.com/antispam) eller ved hjælp af [kommandoen Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Hvis du får vist følgende fejlmeddelelse: **"550 5.7.520 adgang nægtet, din organisation tillader ikke ekstern videresendelse"**, skal du sørge for, at politikken er konfigureret til at aktivere ekstern automatisk videresendelse.

**Bemærk:** Det anbefales, at du holder den eksterne Auto Forward deaktiveret på standardpolitikken for udgående spamfilter og kun aktiverer den for de brugere, der har brug for ekstern videresendelse, ved at oprette en brugerdefineret politik for disse brugere. Du kan læse mere om at [konfigurere ekstern videresendelse af mail i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).