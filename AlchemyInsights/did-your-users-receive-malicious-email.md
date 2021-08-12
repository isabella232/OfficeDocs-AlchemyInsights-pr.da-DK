---
title: Modtog dine brugere skadelig mail
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929191"
---
# <a name="did-your-users-receive-malicious-email"></a>Modtog dine brugere skadelige mails?

- Du kan nu rapportere skadelige mails til Microsoft ved hjælp af [Administrationsindsendelser i Security & Compliance Center.](https://sip.protection.office.com/reportsubmission)

Meddelelser, der sendes i [administratorindsendelser, scannes,](https://sip.protection.office.com/reportsubmission) og følgende resultater vises i pop **op-mailen** med oplysninger:

- Hvis der opstod en fejl i afsenderens mailgodkendelse på leveringstidspunktet.
- Oplysninger om eventuelle politikhits, der kan have påvirket eller tilsidesat konklusionen af en meddelelse.
- Aktuelle detonationsresultater for at se, om URL-adresserne eller filerne i meddelelsen var skadelige eller ej.
- Feedback fra gradere

Hvis der findes en tilsidesættelse, bør genscanning fuldføres efter flere minutter. Hvis der ikke var et problem med mailgodkendelse, eller hvis leveringen ikke blev påvirket af en tilsidesættelse, så kan der gå op til en dags feedback fra gradere.

Hvis du er uenig i den endelige vurdering af en meddelelse, URL-adresse eller fil (blokeret vs. ikke blokeret), skal du sende meddelelsen igen efter en dag for kant. Der er stor risiko for, at konklusionen ændres, når du indsender meddelelsen igen.

I mellemtiden kan du fjerne skadelige mails fra brugernes indbakker ved at følge vejledningen i [denne artikel.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Kunder med Microsoft Defender til Office 365 kan:
    - brug [Trusselsstifinder til at finde og slette mistænkelige mails](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [brug Pengeskab links til at blokere adgangen til](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) en skadelig URL-adresse
    - spor brugere, der klikkede på og fik adgang til skadelige URL-adresser: [Vis phishing-URL-adresse,](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)og klik på  &  [undersøgelsesdataene Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - starte en [automatisk undersøgelse manuelt](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Du kan også beskytte dig mod skadelige filer og URL-adresser ved at følge vejledningen i [Beskyttelse mod skadelige URL-adresser og filer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)