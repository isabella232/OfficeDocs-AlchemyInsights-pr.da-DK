---
title: Mappen 1336 RecoverableItems er fuld
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720246"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen Genoprettes elementer er fuld

For Exchange Online-postkasser er standardlagergrænsen for mappen Genoprettelige elementer 30 GB. Lagergrænsen for mappen Genoprettelige elementer øges automatisk til 100 GB, hvis postkassen placeres i Retslig tilbageholdelse, eDiscovery-tilbageholdelse eller tildeles til en opbevaringspolitik.

Når mappen Genoprettelige elementer når lagergrænsen, påvirkes postkassefunktionaliteten på følgende måder:

- Brugeren kan ikke slette elementer fra postkassen.

- Assistenten til administrerede mapper kan ikke slette elementer baseret på opbevaringskode eller administrerede mappeindstillinger.

- For postkasser, hvor gendannelse af et enkelt element er aktiveret eller er sat i venteposition, kan processen til beskyttelse af siden med kopi-on-write ikke vedligeholde versioner af elementer, der er redigeret af brugeren.

- I forbindelse med postkasser, hvor logføring af postkasseovervågning er aktiveret, kan der ikke gemmes nogen postkasseovervågningslogposter i undermappen Revisioner i mappen Genoprettelige elementer.

I forbindelse med postkasser, der ikke er `Search-Mailbox -SearchDumpsterOnly -DeleteContent` i venteposition, kan administratorer bruge kommandoen i Exchange Online PowerShell til at slette elementer i mappen Genoprettelige elementer. Yderligere oplysninger finder du i følgende emner:

- [Søge efter og slette meddelelser](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Søg-postkasse](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For postkasser, der er i venteposition, skal administratorer fjerne ventepositionen, før de kan slette elementer fra mappen Genoprettelige elementer. Yderligere oplysninger finder du i [Delete items in the Recoverable Items of cloud-based boxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Administratorer kan øge lagergrænsen for mappen Genoprettelige elementer for postkasser i venteposition og konfigurere en politik for opbevaring af postkasser, der flytter elementer fra mappen Genoprettelige elementer til brugerens arkivpostkasse. Se [Øge kvoten For at](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)få postkasser til at gendanne i venteposition .
