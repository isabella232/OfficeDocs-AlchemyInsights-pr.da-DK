---
title: Repliker-sæt
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110674"
---
# <a name="replica-set"></a>Repliker-sæt

AADDS kaldes også for det administrerede domæne. Det er faktisk to domænecontrollere, der køres og vedligeholdes af backend. De to DCs omfatter én hoved-DC og én replikerings-DC. Sikkerhedskopier i AADDS (administreret domæne) er en automatisk proces, der administreres af Azure-platformen. I tilfælde af problemer med dit administrerede domæne kan Azure-support hjælpe dig med at gendanne fra sikkerhedskopien.

Du opretter hvert replikeringssæt i et virtuelt netværk. Hvert virtuelt netværk skal være peered til alle andre virtuelle netværk, der hoster et administreret domænes replikeringssæt. Denne konfiguration opretter en netværktopologi af net, der understøtter katalogreplikering. Et virtuelt netværk kan understøtte flere replikeringssæt, forudsat at hvert replikeringssæt er i et forskelligt virtuelt undernet.

Du kan finde flere oplysninger om Replikeringssæt i [Concepts Replica-sæt](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
