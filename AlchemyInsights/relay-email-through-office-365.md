---
title: Videresend mails via Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324356"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Konfigurer en flerfunktionsenhed eller -program til at sende mail

Se dine muligheder og fremgangsmåden under [Sådan konfigurerer du flerfunktionsenheder eller -programmer til at sende mails ved hjælp af Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Hvis du har en enhed eller et program, der for nyligt er holdt op med at fungere, er de mest almindelige problemer:

- **Godkendelsesrelaterede fejl ved brug af SMTP-godkendt klientindsendelse** Vi har for nylig foretaget nogle ændringer i forbindelse med, hvordan SMTP-godkendelse fungerer. Du kan finde flere oplysninger om, hvordan du løser problemer, i afsnittet Løs problemer med godkendelse uden held i afsnittet Løs problemer med [printere, scannere og LOB-programmer,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)der sender mails ved hjælp af Microsoft 365 eller Office 365.
- **Vi accepterer kun TLS 1.2-versionen, mens vi laver en sikker forbindelse til Office 365** Hvis du bruger en sikker forbindelse (TLS), skal du kontrollere, at din programenhed understøtter TLS 1.2. Du kan finde flere oplysninger [i Forberedelse til TLS 1.2 i Office 365 og Office 365 GCC.](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Du kan finde andre problemer og løsninger under Løse problemer med [printere, scannere](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)og LOB-programmer, der sender mails ved hjælp Microsoft 365 eller Office 365 .

For at se påvirkede enheder skal du gå til [rapporten for SMTP Auth-klienter](https://protection.office.com/mailflow/dashboard).

**Bemærk:** Exchange Online ikke plads til masseforsendelsesscenarier. Hvis du vil sende kommercielle massemails (f.eks. kundebrevbrev), skal du bruge tredjepartsudbydere, der er specialiserede i disse tjenester.
