---
title: 'samme som filnavn er bedst [regel #-beskrivelse]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697124"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Påkrævede Alchemy hovedet H1, H2's virker ikke.
Bedste fremgangsmåder og retningslinjer til oprettelse af Alchemy:

1. **Kan ikke sammensættes Alchemy indblik i mapper**- det ødelægges URL-strukturen. Vi søger til at løse dette.
1. Filerne i mappen **AlchemyInsights** skal have regel-ID og navn på regel fra [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) i filnavnet.
    1. f.eks. ***976-How-to-enable-litigation-hold***
1. Brug metadataene i toppen af denne fil som skabelon. Intet andet er påkrævet.
1. Gå til afsnittet i [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) **kunden indsigt titel:** og brug, der peger som en start til H1 titlen for indsigt. 
    > [!NOTE]
    > Alchemy viden skal have en enkelt H1 øverst eller de brydes i produktionen. H2s gengive ikke, så brug **fed** eller andre konventioner til at angive separate sektioner.
1. Udfyld derefter brødtekst ved hjælp af udkast til materialet i afsnittet kunden indsigt i siden Alchemy regel
    1. Punktopstillede lister er det fint
    1. Nummererede lister for
    1. **Fed** og *kursiv* er a-ok
    1. Links skal altid være en **"links til web" / eksterne** eller **deep-links til elementer i Brugergrænsefladen**, ikke interne hyperlinks.

Og det er virkelig allerede lidt for langt. Den bedste fremgangsmåde er ca 400 tegn---

Når indholdet er klar, kan du trække det til den levende gren. Derefter skal du gå til [Alchemy partnerportal](https://alchemyportal.azurewebsites.net) og indtaste filnavnet i feltet URL-adresse. Kontroller, at indsigt, revideres og offentliggøres, siger "Ja", og klik derefter på Opdater regel. **(Det ser pænere i den nye version af portalen - udgiver snart.)** 
 ![URL-felt](media/for-content-team.PNG)

