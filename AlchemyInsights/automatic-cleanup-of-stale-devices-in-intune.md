---
title: Automatisk oprydning af forældede enheder i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 905881f08ace7afae871ac48fa30ed1a0f15d13972cdff299a6694ca2eafc9cc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997059"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatisk oprydning af forældede enheder i Intune

Intune gør det muligt for administratoren at konfigurere et tidsinterval mellem 90 og 270 dage, hvorefter forældede enheder fjernes fra tjenesten. Denne indstilling gælder for hele organisationen, og når den er aktiveret, træder den i kraft med det samme. Enheder, der ikke er tjekket ind på Intune-serveren i en periode, der overskrider indstillingen, slettes permanent.

**Bemærk!** Kun MDM-enhedsobjekter er berettiget til denne oprydningshandling. Kun EAS-enhedsobjekter udelades.

Du kan få yderligere oplysninger om, hvornår en enhed bliver berettiget til sletning, baseret på enhedens oprydningsindstilling og dens "tilstand":

Indstilling: **Slet enheder efter sidste indtjekningsdato: Ja (noget værdi (N) i angivne dage)**

- Baseret på værdi (N), der er konfigureret i indstillingen, sletter Intune-tjenesten enheden i de angivne dage, efter den sidst blev tjekket ind.

Indstilling:  **Slet enheder efter sidste indtjekningsdato: Nej**

- 180 dage efter enhedscertifikatet udløber og ikke fornyes, slettes enheden.

**Bemærk!** I begge tilfælde skal enheden registreres korrekt i Intune. Registrering sker under den første enhedskontrol med Intune-tjenesten.

Hvis en enhed tilmeldes Intune, men ikke bliver intune registreret, slettes enheden 270 dage efter tilmeldingen. (90 dage til at markere enheden som tilbagekaldt og derefter 180 dage mere til at slette posten).

Der findes i øjeblikket ingen mekanisme i Intune-konsollen til at fastlægge udløbsdatoen for enhedscertificeringen for en given enhed.