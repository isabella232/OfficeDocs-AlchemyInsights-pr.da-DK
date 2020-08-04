---
title: Automatisk oprydning af forældede enheder i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554837"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatisk oprydning af forældede enheder i Intune

Intune gør det muligt for administratoren at konfigurere et tidsinterval mellem 90 og 270 dage, hvorefter forældede enheder fjernes fra tjenesten. Denne indstilling er hele organisationen, og når den er aktiveret, træder den i kraft med det samme. Alle enheder, der ikke er tjekket ind på Intune-serveren i en periode, der overstiger indstillingen, slettes permanent.

**Bemærk:** Det er kun MDM-enhedsobjekter, der er berettiget til denne oprydningshandling. Eas kun enhed objekter er udelukket.

Yderligere oplysninger om, hvornår en enhed bliver berettiget til sletning, er baseret på enhedens oprydningsindstilling og dens "tilstand":

Indstilling: **Slet enheder efter sidste indtjekningsdato: Ja (en vis værdi (N) i angivne dage)**

- Baseret på værdi (N), der er konfigureret i indstillingen, sletter intune-tjenesten enheden i de angivne dage, efter at den sidst er blevet checket ind.

Indstilling: **Slet enheder efter sidste indtjekningsdato: Nej**

- 180 dage efter, at enhedscertifikatet udløber og ikke fornys, slettes enheden.

**Bemærk:** I begge tilfælde skal enheden være registreret i Intune. Registrering sker under den første enheds checkin med Intune-tjenesten.

Hvis en enhed tilmelder sig Intune, men ikke bliver Intune registreret, slettes enheden 270 dage efter tilmeldingen. (90 dage til at markere enheden som tilbagekaldt og derefter yderligere 180 dage til at slette posten).

Der findes i øjeblikket ingen mekanisme i Intune-konsollen til at fastsætte udløbsdatoen for enhedscertificeringen for en given enhed.