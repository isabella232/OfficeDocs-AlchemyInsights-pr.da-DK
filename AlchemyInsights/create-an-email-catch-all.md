---
title: Oprette en mailfangst alle
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286103"
---
# <a name="create-an-email-catch-all"></a>Oprette en mailfangst alle

Brug af en fangst alle er stærkt frarådes. Det er bedre at give en hoppe tilbage til afsenderen lade afsendere vide deres budskab ikke kunne leveres som rettet, så de kan skride til handling. Du kan også begrænse den overvågede postkasse til kun at fange tidligere gyldige e-mailadresser. 

Enhver fangst alle postkasse vil modtage en hel del spam og kan i sidste ende fylde, hvis ikke nøje overvåget. (Der er modtagende grænser). 

Hvis du beslutter dig for at fortsætte, skal du følge disse trin:

1. Opret en dynamisk distributionsgruppe & indeholde "Alle modtagertyper".

2. Opret en dedikeret postkasse for at fange mails, f.catchall@domain.com.

3. Angiv DomainType til "InternalRelay" for det specifikke domæne. Hvis du senere fjerner fangsten alle, skal du sørge for at indstille domænet tilbage til autoritative.

4. Opret en regel for transport af postflow på følgende måde:

    - Hvis afsenderen er "Uden for organisationen"
    - Omdiriger meddelelsen til Catchall@domain.com
    - Undtagen hvis modtageren er medlem af allusers@domain.com (distributionsgruppe indeholder alle medlemmer)
    - Sørg for at validere, at nye postkasser føjes til dynamisk distributionsgruppe
