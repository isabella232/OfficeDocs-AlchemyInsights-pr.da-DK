---
title: Begrænse SharePoint Online til klassisk tilstand
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752062"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begrænse SharePoint Online til klassisk tilstand

Nogle organisationer kræver stadig den klassiske tilstands oplevelse. Selvom der ikke er planer om at fjerne klassisk tilstand på et detaljeret niveau, er det ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.

Administratoren vil have følgende muligheder for at administrere individuelle lister og biblioteker i klassisk tilstand ved hjælp af granulære fravalgs parametre, som vi leverer på følgende niveauer:

- gruppe af websteder
- Websted
- Liste
- Bibliotek

Desuden vil lister, der bruger visse funktioner og tilpasninger, som ikke understøttes af Modern, stadig automatisk blive skiftet til klassisk tilstand.

Begyndende april 1, 2019, den oparbejde hen til forhindre den lejer plan opt op fra moderne liste og biblioteker vil opståen og fortsætte igennem må 31, 2019.  De lister og biblioteker, der er i klassisk tilstand som et resultat af lejer fravalg, vil automatisk blive flyttet til Modern.

Hvis du har brug for klassisk tilstand, skal du se flere oplysninger [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP PowerShell instruktion [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , der beskriver muligheder og værktøjer, du kan bruge i dag til at bruge den klassiske tilstand oplevelse.
