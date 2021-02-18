---
title: Modtog dine brugere skadelig mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291786"
---
# <a name="did-your-users-receive-malicious-email"></a>Modtog dine brugere skadelige mails?

- Du kan nu rapportere den skadelige mail til Microsoft ved hjælp af [administrationsindsendelser i Security & Compliance Center.](https://sip.protection.office.com/reportsubmission)

Meddelelser, der er sendt [i administratorindsendelser, scannes,](https://sip.protection.office.com/reportsubmission) og følgende resultater vises i pop **op-pop op-mailen** med oplysninger:

- Hvis der opstod en fejl i afsenderens mailgodkendelse på leveringstidspunktet.
- Oplysninger om eventuelle politikhits, der kan have påvirket eller tilsidesat konklusionen i en meddelelse.
- Aktuelle detonationsresultater for at se, om URL-adresserne eller filerne i meddelelsen var skadelige eller ej.
- Feedback fra gradere

Hvis der blev fundet en tilsidesættelse, bør genscanning fuldføres på flere minutter. Hvis der ikke var et problem med mailgodkendelse, eller hvis leveringen ikke blev påvirket af en tilsidesættelse, kan det tage op til en dags feedback fra graderne.

Hvis du er uenig i den endelige vurdering af en meddelelse, URL-adresse eller fil (blokeret vs. ikke blokeret), skal du sende meddelelsen igen efter en dag til gennemscanning. Der er stor risiko for, at konklusionen vil blive ændret, når du har sendt meddelelsen igen.

I mellemtiden kan du fjerne ondsindede mails fra brugernes indbakker ved at følge vejledningen i [denne artikel.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Kunder med Microsoft Defender til Office 365 kan:
    - brug [Trusselsstifinder til at finde og slette mistænkelige mails](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [Brug sikre links til at blokere adgangen til](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) en skadelig URL-adresse
    - Spor brugere, der klikkede på og tilgåede ondsindede URL-adresser: [Få vist phishing-URL-adresse,](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)og klik på  &  [advarselsdataene Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - starte en [automatiseret undersøgelse manuelt](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Du kan også beskytte dig mod skadelige filer og URL-adresser ved at følge vejledningen i [Beskyttelse mod skadelige URL-adresser og filer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)