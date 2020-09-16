---
title: Automatisk oprydning af gamle enheder i Intune
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
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715015"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatisk oprydning af gamle enheder i Intune

Intune gør det muligt for administratoren at konfigurere et tidsinterval mellem 90 og 270 dage, hvorefter der fjernes fejl enheder fra tjenesten. Denne indstilling er organisations bredden, og når aktiveret træder i kraft med det samme. Enheder, der ikke er markeret i Intune-serveren for en periode, der overskrider indstillingen, slettes permanent.

**Bemærk!** Kun MDM-enhedsobjekter er berettiget til denne oprydnings handling. Kun EA Device Objects er udeladt.

Du kan finde flere oplysninger om, hvornår en enhed bliver kvalificeret til at blive slettet baseret på indstillingen for oprydning af enheder og dens "tilstand":

Indstilling: **Slet enheder efter sidste checkdato: Ja (nogle af værdierne (N) i dage angivet)**

- Baseret på værdi (N), der er konfigureret i indstillingen, sletter tjenesten Intune enheden i de dage, efter den sidst blev gennemført.

Indstilling:  **Slet enheder efter sidste indtjekning-dato: Nej**

- 180 dage efter at enheds certifikatet udløber og ikke fornys, slettes enheden.

**Bemærk!** I begge tilfælde skal enheden registreres korrekt i Intune. Registrering sker under første enheds indtjekning med Intune-tjenesten.

Hvis en enhed er tilmeldt Intune, men ikke bliver registreret som Intune, slettes enheden 270 dage efter tilmeldingen. (90 dage for at markere enheden som tilbagekaldt og derefter en anden 180 dage for at slette posten.)

Der findes i øjeblikket ingen mekanisme i Intune-konsollen til at oprette udløbsdatoen for enheds certificeringen for en given enhed.