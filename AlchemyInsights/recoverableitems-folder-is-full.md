---
title: 1336 RecoverableItems mappen er fuld
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370381"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen genoprettelige elementer er fuld

For Exchange Online-postkasser i Office 365 er standard lagergrænsen for mappen genoprettelige elementer 30 GB. Lagergrænsen for mappen genoprettelige elementer øges automatisk til 100 GB, hvis postkassen er placeret på tvister Hold eDiscovery hold eller er tildelt en Office 365-opbevaringspolitik.

Når mappen genoprettelige elementer når lagergrænsen, kan postkassen funktionalitet påvirkes på følgende måder:

- Brugeren kan ikke slette elementer fra postkassen.

- En administreret Mappeassistent kan ikke slette elementer baseret på tilbageholdelse kode eller indstillinger for administrerede mapper.

- Ikke for postkasser, der er enkelt vare genoprettelse aktiveret eller er sat i venteposition, vedligeholde kopier ved skrivning-side beskyttelse processen versioner af elementer, der er redigeret af brugeren.

- For postkasser, der har en postkasse Overvåg logføring er aktiveret, kan ingen postkasse overvågningsposter log gemmes i audit-undermappe i mappen genoprettelige elementer.

Administratorer kan bruge til postkasser, der ikke er på hold, den `Search-Mailbox -SearchDumpsterOnly -DeleteContent` i Exchange Online PowerShell til at slette elementer i mappen genoprettelige elementer. Yderligere oplysninger finder du i følgende emner:

- [Søge efter og slette meddelelser](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Søg-postkasse](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Administratorer har for postkasser, der er sat på hold, til at fjerne spærringen, før de kan slettede elementer fra mappen genoprettelige elementer. Yderligere oplysninger finder du under [slette emner i mappen skybaserede postkasser på hold genoprettelige elementer](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

For at forhindre, at mappen genoprettelige elementer bliver fuld, kan administratorer øge lagergrænsen genoprettelige elementer mappe til postkasser på hold og konfigurere en postkasse opbevaringspolitik, som flytter elementer fra mappen genoprettelige elementer til brugerens arkiv postkasse. Se [øge genoprettelige elementer kvote for postkasser på hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
