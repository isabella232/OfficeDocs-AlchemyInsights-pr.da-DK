---
title: Repliker sæt
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
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713750"
---
# <a name="replica-set"></a>Repliker sæt

AADDS kaldes også for det administrerede domæne. Det er faktisk to domænecontrollere, der køres og vedligeholdes af backend. De to DCs omfatter én hoved-DC og én replikerings-DC. Sikkerhedskopier i AADDS (administreret domæne) er en automatiseret proces, der administreres af Azure-platformen. I tilfælde af et problem med dit administrerede domæne kan Azure-support hjælpe dig med at gendanne fra sikkerhedskopien.

Du opretter hvert replikeringssæt i et virtuelt netværk. Hvert virtuelt netværk skal peeres til alle andre virtuelle netværk, der hoster et administreret domænes replikeringssæt. Denne konfiguration opretter en netværktopologi til net, der understøtter katalogreplikering. Et virtuelt netværk kan understøtte flere replikeringssæt, forudsat at hvert replikeringssæt er i et andet virtuelt undernet.

Du kan finde flere oplysninger om replikeringssæt i [Concepts Replica-sæt.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
