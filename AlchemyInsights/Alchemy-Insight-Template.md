---
title: samme som filnavn er bedst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800039"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Påkrævet Alchemy header H1, H2's dont arbejde.
Bedste fremgangsmåder og retningslinjer for Alchemy authoring:

1. **Du må ikke indlejre Alchemy Insights i mapper**-dette vil bryde URL-strukturen. Vi kigger på at ordne det her.
1. Filer i mappen **Alchemyinsights** skal have små filnavne med bindestreger til mellemrum ex. ***Sådan gør du-aktiver-retssager-hold***.
    1. Medtag regel-id'et eller bucket-id'et fra [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net) i MS. Custom-feltet. Ex. ***MS. Custom: 100021***
1. Brug resten af metadataene øverst i denne fil som skabelon.
1. I [Alchemy partner portalen](https://alchemyportal.azurewebsites.net)skal du navigere ned til afsnittet **kunde Insight-titel:** og bruge det som udgangspunkt for din H1-titel til indsigten. 
    > [!NOTE]
    > Alchemy Insights skal kun have en enkelt H1 i toppen, eller de vil bryde i produktionen. H2S Render ikke enten så brug **fed** eller andre konventioner til at betyde separate sektioner.
1. Udfyld derefter brødteksten ved hjælp af kladde materialet i afsnittet Kundeindsigt på siden Alchemy Rule
    1. Punktopstillinger er fine
    1. Nummererede lister også
    1. **Fed** og *kursiv* er a-OK
    1. Links skal altid være enten **"links til web"/eksterne** eller **dybe-links til UI elementer**, ikke interne links.
    1. Billeder er ikke officielt understøttet på dette tidspunkt, men det er på køreplanen.

Og det er virkelig allerede lidt for længe. Bedste praksis er omkring 400 tegn---------------------------------

Når dit indhold er klar, skal du trække det til live grenen. Gå derefter til [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net) , og Indtast filnavnet i URL-feltet. 