---
title: 1336 RecoverableItems-mappen er fuld
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741261"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen Genoprettelige elementer er fuld

For Exchange Online-postkasser er standardlager grænsen for mappen Genoprettelige elementer 30 GB. Lagergrænsen for mappen Genoprettelige elementer øges automatisk til 100 GB, hvis postkassen er placeret i retssag, eDiscovery-venteposition eller er tildelt en opbevaringspolitik.

Når mappen Genoprettelige elementer Når lagergrænsen, påvirkes postkasse funktionaliteten på følgende måder:

- Brugeren kan ikke slette elementer fra postkassen.

- Assistent til administrerede mapper kan ikke slette elementer, der er baseret på opbevarings kode eller indstillinger for administrerede mapper.

- For postkasser, hvor en enkelt element gendannelse er aktiveret eller er sat i venteposition, kan der ikke gemmes versioner af de elementer, der er blevet redigeret af brugeren.

- For postkasser, hvor logføring for postkasse overvågning er aktiveret, kan der ikke gemmes nogen poster til overvågningslogfiler for postkassen i under mappen reitems i Genoprettelige elementer.

For postkasser, der ikke er i venteposition, kan administratorer bruge `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til at slette elementer i mappen Genoprettelige elementer. Hvis du vil have mere at vide, skal du se følgende emner:

- [Søg efter og slet meddelelser](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Søg-postkasse](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For postkasser, der er i venteposition, skal administratorer fjerne ventepositionen, før de kan slette elementer fra mappen Genoprettelige elementer. Hvis du vil have mere at vide, skal du se [Slet elementer i mappen Genoprettelige elementer i skybaserede postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

For at forhindre, at mappen Genoprettelige elementer bliver fuld, kan administratorer øge lagergrænsen for mappen Genoprettelige elementer for postkasser i venteposition og konfigurere en opbevaringspolitik for postkasser, der flytter elementer fra mappen Genoprettelige elementer til brugerens Arkiv postkasse. Se [Forøg kvoten for Genoprettelige elementer for postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
