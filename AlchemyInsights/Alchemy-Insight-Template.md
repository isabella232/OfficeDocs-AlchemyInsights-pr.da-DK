---
title: det samme som filnavnet er bedst
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
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664128"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Påkrævet Alchemy-sidehoved H1, H2's virker ikke."
Bedste fremgangsmåder og retningslinjer for Alchemy-redigering:

1. **Du må ikke indlejre Alchemy-indsigt i mapper**– dette bryder URL-strukturen ud. Vi er ved at rette dette.
1. Filer i mappen **AlchemyInsights** skal have små filnavne med bindestreger for mellemrum. ***Sådan aktiverer du en retssag***.
    1. Medtag regel-ID eller Bucket-ID fra [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net) i MS. brugerdefineret felt. udvidet. ***MS. Custom: 100021***
1. Brug resten af metadataene øverst i denne fil som skabelon.
1. I [Alchemy-partner portalen](https://alchemyportal.azurewebsites.net)skal du gå til afsnittet **kundens indblikings titel:** og bruge det som udgangspunkt for din H1-titel for indsigt. 
    > [!NOTE]
    > Alchemy indsigt må kun have et enkelt H1 øverst, eller de vil bryde op i produktion. H2S gengives ikke, så brug af **fed** eller andre konventioner til at angive separate sektioner.
1. Derefter skal du udfylde brødteksten ved hjælp af kladde materialet i sektionen kunde indsigt på Alchemy-regel siden
    1. Punktopstillinger er fine
    1. Nummererede lister
    1. **Fed** og *kursiv* er en-OK
    1. Links bør altid være **"links til internettet"-/External** eller **dyb links til brugergrænsefladeelementer**, ikke interne kæder.
    1. Billeder er ikke officielt understøttet på nuværende tidspunkt, men det er på køreplanen.

Og det er meget, at det allerede er lidt for langt. Den bedste fremgangsmåde handler om 400 tegn---------------------------------

Når dit indhold er klar, skal du trække det til den direkte forgrening. Gå derefter til Alchemy- [partner portalen](https://alchemyportal.azurewebsites.net) , og Indtast filnavnet i feltet URL-adresse. 