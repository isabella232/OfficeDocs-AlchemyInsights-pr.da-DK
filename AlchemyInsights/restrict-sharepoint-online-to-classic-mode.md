---
title: Begræns SharePoint Online til klassisk tilstand
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742463"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begræns SharePoint Online til klassisk tilstand

Nogle organisationer kræver stadig den klassiske tilstandsoplevelse. Selvom der ikke er planer om at fjerne klassisk tilstand på et detaljeret niveau, er det ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.

Administratoren har følgende muligheder for at administrere individuelle lister og biblioteker i klassisk tilstand ved hjælp af detaljerede fravalgsparametre, som vi leverer på følgende niveauer:

- gruppe af websteder
- Websted
- Liste
- Bibliotek

Derudover vil lister, der bruger bestemte funktioner og tilpasninger, der ikke understøttes af moderne, stadig automatisk blive skiftet til klassisk tilstand.

april 2019 starter processen med at deaktivere lejerniveaufravalg af moderne liste og biblioteker frem til 31. maj 2019.  De lister og biblioteker, der er i klassisk tilstand som følge af lejer opt-out, vil automatisk blive flyttet til moderne.

Hvis du har brug for klassisk tilstand kan du se mere information [her](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) og PnP Powershell instruktion [her,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) der beskriver muligheder og værktøjer, du kan bruge i dag til at bruge den klassiske tilstand oplevelse.
