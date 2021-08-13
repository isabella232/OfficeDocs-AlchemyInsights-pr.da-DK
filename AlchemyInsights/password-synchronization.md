---
title: Synkronisering af adgangskoder
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960829"
---
# <a name="password-synchronization"></a>Synkronisering af adgangskoder

**Synkronisering af adgangskodehash virker slet ikke**

Nogle almindelige problemer, som kunder støder på, når synkronisering af adgangskodehash ikke virker, er:

- Active Directory-kontoen, der bruges af Azure AD Forbind til at kommunikere  med Active Directory i det lokale miljø, får ikke tildelt Repliker mappeændringer og **Repliker** mappeændringer Alle tilladelser, som er nødvendige for synkronisering af adgangskoder – Det er du nødt til at løse ved at give disse tilladelser til Active Directory-kontoen.
- Synkronisering af adgangskodehash er deaktiveret, når  en administrator har ændret metoden User Sign-In fra Synkronisering af adgangskoder til en anden indstilling, f.eks. Sammenslutning med **AD FS** i Azure AD Forbind-guiden – Du kan løse dette problem ved at genaktivere funktionen til synkronisering af adgangskodehash i Azure AD Forbind-guiden. 
- Forbindelsesproblem med Active Directory i det lokale miljø. Nogle domænecontrollere er f.eks. ikke tilgængelige for [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Forbind, eller de påkrævede porte er blokeret af Firewall – det skal du løse ved at sikre, at forbindelsen mellem Azure AD Forbind-serveren og den lokale Active Directory fungerer korrekt.
- Azure AD Forbind-serveren er i i øjeblikket i iscenesættelsestilstand, hvilket medfører, at serveren ikke kan udføre adgangskodehashes – Hvis du vil foretage fejlfinding af problemet, skal du følge de trin, der er beskrevet i Fejlfinding i forbindelse med synkronisering af adgangskoder med Azure AD Forbind - Ingen adgangskoder [synkroniseres.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Synkronisering af adgangskodehash virker ikke for nogle af mine brugere**

1. Hvis du har bemærket, at adgangskodehash ikke  synkroniseres for en bruger, kan du bruge fejlfindingsopgaven i Azure AD Forbind til at undersøge og løse problemet. Udfør følgende opgaver:

    a. [Kør fejlfindingsopgaven i guiden](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Brug fejlfindings-cmdlet'en til at undersøge synkroniseringen af adgangskodehash for en bestemt brug](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Det lokale Active Directory-brugerobjekt er aktiveret for **brugeren, og brugeren skal ændre adgangskoden ved næste logonindstilling.** Når denne indstilling er aktiveret, tildeles brugeren en midlertidig adgangskode og bliver bedt om at ændre adgangskoden ved næste logon. Azure AD Forbind synkroniserer ikke midlertidige adgangskoder til Azure AD.

Du kan løse problemet ovenfor ved at udføre en af følgende opgaver:

- Bed brugeren om at logge på det lokale program (f.eks Windows Desktop) og ændre adgangskoden. Den nye adgangskode synkroniseres med Azure AD.
- Få en administrator til at opdatere brugerens adgangskode uden at aktivere indstillingen Brugeren skal ændre adgangskoden ved næste **logon** og dele den nye adgangskode med brugeren.

3. Det lokale Active Directory-brugerobjekt er ikke **konfigureret korrekt** til objektsynkronisering eller synkronisering af adgangskoder. Hvis du vil foretage fejlfinding af dette problem, skal du følge de trin, der er beskrevet i Fejlfinding af synkronisering af [adgangskodehash med Azure AD Forbind synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







