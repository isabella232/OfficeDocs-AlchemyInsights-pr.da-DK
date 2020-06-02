---
title: 1336 Mappen RecoverableItems er fuld
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
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510746"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen Genopretteligt elementer er fuld

For Exchange Online-postkasser er standardlagergrænsen for mappen Genoprettelige elementer 30 GB. Lagergrænsen for mappen Genoprettelige elementer øges automatisk til 100 GB, hvis postkassen placeres i Retslig tilbageholdelse, eDiscovery-venteposition eller er tildelt til en opbevaringspolitik.

Når mappen Genoprettelige elementer når lagergrænsen, påvirkes postkassefunktionaliteten på følgende måder:

- Brugeren kan ikke slette elementer fra postkassen.

- Assistenten for administrerede mapper kan ikke slette elementer baseret på indstillinger for opbevaringskode eller administrerede mapper.

- For postkasser, hvor gendannelse af enkeltelement er aktiveret eller er sat i venteposition, kan sidebeskyttelsesprocessen for copy-on-write ikke vedligeholde versioner af elementer, der er redigeret af brugeren.

- For postkasser, hvor postkasseovervågningslogføring er aktiveret, kan der ikke gemmes poster i undermappen Overvågning i undermappen Overvågning i mappen Genoprettelige elementer.

I forbindelse med postkasser, der ikke er i venteposition, kan administratorer bruge `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til at slette elementer i mappen Genoprettelige elementer. Yderligere oplysninger finder du i følgende emner:

- [Søge efter og slette meddelelser](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Søg-postkasse](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

I forbindelse med postkasser, der er i venteposition, skal administratorer fjerne ventepositionen, før de kan slette elementer fra mappen Genoprettelige elementer. Du kan finde flere oplysninger [under Slette elementer i mappen Genoprettelige elementer i skybaserede postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Administratorer kan øge lagergrænsen for mappen Genoprettelige elementer for postkasser, der er i venteposition, og oprette en politik for opbevaring af postkasser, der flytter elementer fra mappen Genoprettelige elementer til brugerens arkivpostkasse. Se [Øge kvoten for elementer, der kan gendannes, for postkasser i venteposition](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
