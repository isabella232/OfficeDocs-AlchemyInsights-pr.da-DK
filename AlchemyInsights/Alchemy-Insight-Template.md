---
title: samme som filnavn et bedst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676527"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Krævet Alkymi Header H1, H2's virker ikke.
Bedste fremgangsmåder og retningslinjer for Alkymi authoring:

1. **Må ikke reden Alchemy Insights i mapper**- dette vil bryde url struktur. Vi undersøger, hvordan vi løser det her.
1. Filer i mappen **AlchemyInsights** skal have filnavne med små bogstaver med bindestreger til mellemrum f.eks. ***how-to-enable-litigation-hold***.
    1. Medtag regel-id'et eller bucket-id'et fra [Alkymy Partner-portalen](https://alchemyportal.azurewebsites.net) i feltet ms.custom. Ex. ***ms.custom: 100021***
1. Brug resten af metadataene øverst i denne fil som skabelon.
1. I [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net)skal du navigere ned til afsnittet **Customer Insight-titel:** og bruge den som udgangspunkt for din H1-titel for indsigten. 
    > [!NOTE]
    > Alkymi Insights SKAL kun have en enkelt H1 øverst, eller de vil bryde i produktionen. H2'er gengives ikke, så brug **fed** eller andre konventioner til at betyde separate sektioner.
1. Udfyld derefter brødteksten ved hjælp af kladdematerialet i afsnittet Kundeindsigt på siden Alkymiregel
    1. Punktopstillinger er fine
    1. Nummererede lister også
    1. **Fed** og *kursiv* er a-ok
    1. Links bør altid være enten **"links til web"/eksterne** eller **dybe links til elementer i brugergrænsefladen**, ikke interne links.
    1. Billeder er ikke officielt understøttet på nuværende tidspunkt, men det er på køreplanen.

Og det er virkelig allerede lidt for længe. Bedste praksis er omkring 400 tegn ---------------------------------

Når dit indhold er klar, skal du trække det til den levende gren. Gå derefter til [Alchemy Partner-portalen,](https://alchemyportal.azurewebsites.net) og angiv filnavnet i url-feltet. 