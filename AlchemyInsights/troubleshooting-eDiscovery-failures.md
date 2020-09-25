---
title: 1490 – fejlfinding – eDiscovery-fejl
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277813"
---
# <a name="troubleshoot-content-search-errors"></a>Fejlfinding af indholds søgefejl

Oplever du problemer med at søge efter indhold eller få fejl, når du eksporterer søgeresultater?

For eksempel modtager du følgende, når du kører søgninger?

- CS008-eller CS012-fejl

- Fejl på serveren er optaget/timeout

- Der opstod en programfejl

Eller når du søger efter eller eksporterer resultater fra et stort antal postkasser (over 100.000-postkasser), får du eksport fejl?

For disse fejltyper kan du prøve at søge efter de indholdssteder, der er mislykket. Du kan finde flere oplysninger i  [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Hvis du eksporterer mere end 100K-postkasser, skal du bruge følgende PowerShell til at downloade eksportresultaterne:  [eksportere resultater fra mere end 100K postkasser](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
