---
title: Skift af Yammer-standarddomæne for Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 93c82b7e60838e0127062e8bf5ab394bb29650d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793860"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Skift af standard-/primært Yammer-domæne

Yammer URL-adressen indeholder det aktuelle primære domænenavn for dit Yammer-netværk. Dette domænenavn svarer muligvis ikke til det primære domænenavn, der er valgt i Office 365 eller Azure AD. Der er forskelle i adfærd baseret på antallet af brugerdefinerede domæner, der er føjet til lejeren, og om Yammer er i en understøttet konfiguration (1 lejer: 1 netværk eller 1:1). Der findes dokumentation på [Yammer-domæner og Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Den mest almindelige årsag til, at du ser et forkert domæne, er, at der findes flere Yammer-netværk, og de skal konsolideres. [Konsolidering til et enkelt netværk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ved hjælp af værktøjet til netværksoverførsel er et vigtigt første trin. Udfør dette, før du forsøger at angive dit primære domæne.

**Ingen brugerdefinerede domæner**

For nye lejere vil standarddomænet (f.eks. fabrikam.onmicrosoft.com) fra lejeren blive brugt til Yammer. Det primære domæne er indstillet til yammer.com/fabrikam.onmicrosoft.com.

**Enkelt brugerdefineret domæne**

Yammer vil automatisk vælge det brugerdefinerede domæne (f.eks. fabrikam.com) fra lejeren som det primære domæne i Yammer. Det er indstillet til yammer.com/fabrikam.com. Denne ændring foretages af tjenesten til domænesynkronisering, og kan tage op til 24 timer at træde i kraft.

**Flere brugerdefinerede domæner**

Yammer kan have et primært domæne, der er forskelligt fra det standard lejerdomæne. Da der er flere brugerdefinerede domæner, forsøger Yammer ikke at gætte det rigtige domæne ud fra de tilgængelige. Du skal åbne en supportsag for at anmode om, at det primære domænenavn ændres til det primære domæne efter eget valg.

**Yderligere fejlfindingsoplysninger**

I nogle tilfælde kan domæner være blevet flyttet mellem lejere, og tjenesten til domænesynkronisering kan ikke køre korrekt. Du kan opleve logon- eller andre problemer, foruden et forkert primært domæne. For at løse dette problem kan domæner være nødt til at blive flyttet til det rigtige netværk med hjælp fra Microsoft Support. Denne situation kræver direkte hjælp, og det kan tage lidt tid at løse problemet, især hvis der er en meget lang liste med domænenavne. Åbn en supportsag, hvis du vil have hjælp til at løse disse typer problemer.

Når du arbejder med en supportmedarbejder, kontrollerer de, om domæner er bekræftet på en lejer, som du styrer. De kan stille yderligere bekræftelsesspørgsmål om dine domæner, hvis de er føjet til din lejer, men ikke bekræftet af DNS. Sørg for, at domæner er bekræftet af DNS for at fremskynde processen.
