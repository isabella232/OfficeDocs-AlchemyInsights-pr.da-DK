---
title: samme som filnavn er bedst
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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750964"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Krævede Alkymi Header H1, H2's virker ikke."
Bedste fremgangsmåder og retningslinjer for alkymi authoring:

1. **Må ikke indlejre Alchemy Insights i mapper**- dette vil bryde url struktur. Vi undersøger, om vi skal ordne det her.
1. Filer i mappen **AlchemyInsights** skal have filnavne med små bogstaver med bindestreger til mellemrum ex. ***hvordan-til-aktivere-retssager-hold***.
    1. Medtag regel-id'et eller bucket-id'et fra [alkymipartnerportalen](https://alchemyportal.azurewebsites.net) i ms.custom-feltet. Ex. ***ms.custom: 100021***
1. Brug resten af metadataene øverst i denne fil som skabelon.
1. På [Alchemy Partner-portalen skal](https://alchemyportal.azurewebsites.net)du navigere ned til afsnittet **Customer Insight Title:** og bruge det som udgangspunkt for din H1-titel til indsigten. 
    > [!NOTE]
    > Alkymi Insights SKAL kun have en enkelt H1 i toppen, eller de vil bryde i produktionen. H2s ikke gøre enten så brug **fed** eller andre konventioner til at betyde separate sektioner.
1. Udfyld derefter brødteksten ved hjælp af kladdematerialet i afsnittet Kundeindsigt på siden Alchemy Rule
    1. Punktopstillinger er fine
    1. Også opstilling af tal/bogstaver
    1. **Fed** og *kursiv* er a-ok
    1. Links bør altid være enten **"links til web"/eksterne** eller **dybe links til UI elementer,** ikke interne links.
    1. Billeder er ikke officielt understøttet på nuværende tidspunkt, men det er på køreplanen.

Og det er virkelig allerede lidt for længe. Bedste praksis er omkring 400 tegn ---------------------------------

Når dit indhold er klar, skal du trække det til live grenen. Gå derefter til [Alchemy Partner-portalen,](https://alchemyportal.azurewebsites.net) og indtast filnavnet i url-feltet. 