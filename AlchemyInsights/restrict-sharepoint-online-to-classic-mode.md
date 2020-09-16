---
title: Begræns SharePoint Online til klassisk tilstand
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751416"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begræns SharePoint Online til klassisk tilstand

Nogle organisationer kræver stadig den klassiske oplevelse af tilstanden. Selvom der ikke er nogen planer om at fjerne klassisk tilstand på et detaljeret niveau, er det ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.

Administratoren har følgende muligheder for at administrere individuelle lister og biblioteker i klassisk tilstand med detaljerede afleverings parametre, som vi giver på følgende niveauer:

- gruppe af websteder
- adresse
- liste
- bibliotek

Desuden vil lister, der bruger visse funktioner og tilpasninger, der ikke understøttes af moderne, stadig automatisk skifte til klassisk tilstand.

Startende 1, 2019, processen til deaktivering af det lejerniveau, du har logget af moderne liste og biblioteker, starter og fortsætter gennem maj 31, 2019.  De lister og biblioteker, der er i klassisk tilstand som resultat af lejerens lejer, bliver automatisk videre hævet til moderne.

Hvis du har brug for klassisk tilstand, skal du se flere oplysninger [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP PowerShell-instruktion [her](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , der beskriver indstillinger og værktøjer, du kan bruge i dag for at bruge den klassiske oplevelse af tilstanden.
