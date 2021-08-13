---
title: 1336-mappen GenopretteligeWebsteder er fuld
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061750"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen med genoprettelige elementer er fuld

For Exchange Online postkasser er standardlagergrænsen for mappen Genoprettelige elementer 30 GB. Lagergrænsen for mappen Genoprettelige elementer øges automatisk til 100 GB, hvis postkassen er placeret i Retslig tilbageholdelse, eDiscovery-venteposition eller er tildelt en opbevaringspolitik.

Når mappen Genoprettelige elementer når lagergrænsen, påvirkes postkassefunktionaliteten på følgende måder:

- Brugeren kan ikke slette elementer fra postkassen.

- Administreret mappeassistent kan ikke slette elementer baseret på opbevaringsmærke eller administrerede mappeindstillinger.

- For postkasser, der har aktiveret gendannelse af enkeltelement eller er sat i venteposition, kan beskyttelsesprocessen for kopiér-på-skriv-siden ikke vedligeholde versioner af elementer, der er redigeret af brugeren.

- For de postkasser, hvor logføring af postkassekontrol er aktiveret, kan ingen poster i postkassens overvågningslog gemmes i undermappen Revision i mappen Genoprettelige elementer.

For postkasser, der ikke er i venteposition, kan administratorer bruge kommandoen i Exchange Online PowerShell til at slette elementer i mappen `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Genoprettelige elementer. Du kan finde flere oplysninger i følgende emner:

- [Søge efter og slette meddelelser](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For postkasser, der er i venteposition, skal administratorer fjerne ventepositionen, før de kan slette elementer fra mappen Genoprettelige elementer. Få mere at vide under [Slet elementer i mappen Genoprettelige elementer i skybaserede postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

For at forhindre mappen Genoprettelige elementer i at blive fuld, kan administratorer øge lagergrænsen for mappen Genoprettelige elementer for postkasser i venteposition og konfigurere en opbevaringspolitik for postkasser, der flytter elementer fra mappen Genoprettelige elementer til brugerens arkivpostkasse. Se [Øg kvoten for genoprettelige elementer for postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
