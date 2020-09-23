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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219849"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokere eller fjerne blokeringen af videresendelse af mail

Hvis du vil aktivere eller deaktivere videresendelse af mail for en bestemt postkasse, skal du se [konfigurere videresendelse af mail](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

På lejerniveau foretages kontrol af ekstern videresendelse ved hjælp af udgående politik om uønsket post. Hvis den er indstillet til fra eller automatisk, kan det blokere for videresendelse af mails med "550 5.7.520 adgang nægtet, din organisation tillader ikke ekstern videresendelse". Hvis viderestilling blev angivet til at blive blokeret, så er den fejl, brugerne får vist.

Hvis videresendelse blokeres, skal du kontrollere, at politikken er konfigureret til at aktivere ekstern Auto Forward. Du kan kontrollere politikken for udgående spam filter fra sikkerheds-og overholdelses Center eller ved at køre kommandoen Get-HostedOutboundSpamFilterPolicy | fl-navn, AutoForwardingMode. Hvis du vil konfigurere blokering af viderestilling af autoforward, vil den samme kommando fortælle dig, at politiktilstanden nu.

Bemærk! det anbefales, at du holder den eksterne Auto Forward deaktiveret på standardpolitikken for udgående spam filter og kun aktiverer den for de brugere, der har brug for ekstern videresendelse, ved at oprette en brugerdefineret politik for disse brugere. Du kan læse mere om at [konfigurere ekstern videresendelse af mail i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).