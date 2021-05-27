---
title: Softwarelager mangler eller er unøjagtigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676142"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Softwarelager mangler eller er unøjagtigt

Softwarelageret på Håndtering af trusler og sikkerhedsrisici (TVM) er en liste over kendt software i din organisation med officielle Common Platform Enumerations (CPE).

Softwareprodukter uden en officiel CPE har ikke offentliggjort sårbarheder. Lageret indeholder også oplysninger som f.eks. navnet på leverandøren, antallet af personer, trusler og antallet af enheder, der vises.

Softwareændringer på enheder afspejles typisk i sikkerhedsportaler inden for to timer. Men det kan nogle gange tage længere tid. Det er i øjeblikket ikke muligt at gennemtvinge en synkronisering. dette er en løbende løbende vurdering.

Hvis du har foretaget en softwareændring, og ændringen ikke afspejles nøjagtigt i TVM efter 5 timer, skal du følge disse trin:

1. Kontrollér afsnittet om software beviser for at forstå, hvordan softwaren blev registreret.
1. Sørg for, at softwaren understøttes. Software kan kun ses på enhedsniveau, selvom det i øjeblikket ikke understøttes af Håndtering af trusler og sikkerhedsrisici. Men kun begrænsede data er tilgængelige.
1. Du kan finde en vejledning til, hvordan du rapporterer unøjagtigheden fra portalen, [under Rapport om unøjagtighed.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **Bemærk!** Rapportering af en unøjagtighed fra MDE-portalen er en envejskanal til tekniker. Hvis problemet haster, skal du åbne en supportanmodning.

Du kan finde flere oplysninger [i Softwarelager – Håndtering af trusler og sikkerhedsrisici](/microsoft-365/security/defender-endpoint/tvm-software-inventory).