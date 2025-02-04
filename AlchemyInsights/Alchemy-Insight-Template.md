---
title: det samme som filnavn er bedst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312819"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Påkrævet Alchemy Header H1, H2 virker ikke."
Bedste fremgangsmåder og retningslinjer for alchemy-redigering:

1. **Du må ikke indlejre Alchemy Insights i mapper**– dette vil bryde URL-strukturen. Vi er ved at løse dette.
1. Filer i mappen **AlchemyInsights** skal have små filnavne med bindestreger for mellemrum f.eks. **_how-to-enable-litigation-hold_**.
    1. Medtag regel-id'et eller [bucket-id'et fra Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net) i det ms.custom felt. f.eks. ***ms.custom: 100021***
1. Brug resten af metadataene øverst i denne fil som din skabelon.
1. I [Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net)skal du  gå ned til afsnittet Kundeindsigtstitel: og bruge det som et udgangspunkt for din H1-titel til indsigten. 

**Bemærk!** Alchemy Insights SKAL kun have en enkelt H1 øverst, ellers afbrydes produktion. H2-værdier gengives hverken, så brug **fed eller** andre konventioner til at signere separate sektioner.
1. Udfyld derefter brødteksten ved hjælp af kladdematerialet i Customer Insights på siden Alchemy Rule
    1. Opstillinger med punkttegn er fine
    1. Også nummererede lister
    1. **Fed** og *kursiv* er a-ok
    1. Links skal altid være enten **"links til web"/eksterne** ELLER **dybe links til brugergrænsefladeelementer** og ikke interne links.
    1. Billeder understøttes ikke officielt på nuværende tidspunkt, men de er på vej.

Og det er i virkeligheden allerede lidt for lang. Bedste fremgangsmåde er ca. 400 tegn ---------------------------------

Når dit indhold er klar, skal du trække det til live-grenen. Gå derefter til [Alchemy-partnerportalen,](https://alchemyportal.azurewebsites.net) og angiv filnavnet i url-feltet. 