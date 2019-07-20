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
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800039"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Påkrævede Alchemy hovedet H1, H2's virker ikke.
Bedste fremgangsmåder og retningslinjer til oprettelse af Alchemy:

1. **Kan ikke sammensættes Alchemy indblik i mapper**- det ødelægges URL-strukturen. Vi søger til at løse dette.
1. Filerne i mappen **AlchemyInsights** skal have små filnavne med bindestreger i mellemrum ex. ***how-til-aktivere-retssag-hold***.
    1. Omfatte regel-ID eller bucket-ID fra [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) i feltet ms.custom. ex. ***MS.Custom: 100021***
1. Brug resten af metadataene i toppen af denne fil som skabelon.
1. Gå til afsnittet i [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) **kunden indsigt titel:** og brug, der peger som en start til H1 titlen for indsigt. 
    > [!NOTE]
    > Alchemy viden skal have en enkelt H1 øverst eller de brydes i produktionen. H2s gengive ikke, så brug **fed** eller andre konventioner til at angive separate sektioner.
1. Udfyld derefter brødtekst ved hjælp af udkast til materialet i afsnittet kunden indsigt i siden Alchemy regel
    1. Punktopstillede lister er det fint
    1. Nummererede lister for
    1. **Fed** og *kursiv* er a-ok
    1. Links skal altid være en **"links til web" / eksterne** eller **deep-links til elementer i Brugergrænsefladen**, ikke interne hyperlinks.
    1. Billeder understøttes ikke officielt på nuværende tidspunkt, men det er i gang med køreplanen.

Og det er virkelig allerede lidt for langt. Den bedste fremgangsmåde er ca 400 tegn---

Når indholdet er klar, kan du trække det til den levende gren. Derefter skal du gå til [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) og indtaste filnavnet i feltet URL-adresse. 