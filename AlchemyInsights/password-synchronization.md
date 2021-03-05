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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481444"
---
# <a name="password-synchronization"></a>Synkronisering af adgangskoder

**Synkronisering af adgangskodehash virker slet ikke**

Nogle almindelige problemer, som kunder støder på, når synkronisering af adgangskodehash ikke virker, er:

- Active Directory-kontoen, der bruges af Azure AD Connect til at kommunikere med Active Directory i det lokale miljø, tildeles ikke **Repliker** mappeændringer og **Repliker** mappeændringer Alle tilladelser, som er nødvendige for synkronisering af adgangskoder – Du skal løse dette problem ved at give disse tilladelser til Active Directory-kontoen.
- Synkronisering af adgangskodehash er deaktiveret, efter  at en administrator har ændret metoden Bruger Sign-In fra Synkronisering af adgangskode til en anden  indstilling, f.eks. Sammenslutning med **AD FS,** i Azure AD Connect-guiden . Du kan løse dette problem ved at genaktivere funktionen til synkronisering af adgangskodehash i azure AD Connect-guiden.
- Forbindelsesproblem med Active Directory i det lokale miljø. Nogle domænecontrollere er f.eks. ikke tilgængelige [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) for Azure AD Connect, eller de påkrævede porte er blokeret af Firewall – du skal løse dette problem ved at sikre, at forbindelsen mellem Azure AD Connect-serveren og den lokale Active Directory fungerer korrekt.
- Azure AD Connect-serveren befinder sig i øjeblikket i midlertidig tilstand, hvilket medfører, at serveren ikke kan bruge adgangskodehashes – Hvis du vil foretage fejlfinding af problemet, skal du følge de trin, der er beskrevet i afsnittet Fejlfinding i forbindelse med synkronisering af adgangskoder med [Azure AD Connect-synkronisering –](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Der synkroniseres ingen adgangskoder.

**Synkronisering af adgangskodehash fungerer ikke for nogle af mine brugere**

1. Hvis du har bemærket, at adgangskodehash ikke  synkroniseres for en bruger, kan du bruge fejlfindingsopgaven i Azure AD Connect til at undersøge og løse problemet. Udfør følgende opgaver:

    a. [Kør fejlfindingsopgaven i guiden](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Brug fejlfindings-cmdlet'en til at undersøge synkroniseringsproblemet med adgangskodehash til en bestemt brug](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Det lokale Active Directory-brugerobjekt er aktiveret for **brugeren, og adgangskoden skal ændres ved næste logonindstilling.** Når denne indstilling er aktiveret, får brugeren tildelt en midlertidig adgangskode og bliver bedt om at ændre adgangskoden ved næste logon. Azure AD Connect synkroniserer ikke midlertidige adgangskoder til Azure AD.

Du kan løse problemet herover ved at udføre en af følgende opgaver:

- Bed brugeren om at logge på det lokale program (f.eks. Skrivebordsversionen af Windows) og ændre adgangskoden. Den nye adgangskode synkroniseres med Azure AD.
- Få en administrator til at opdatere brugerens adgangskode uden at aktivere indstillingen Brugeren skal ændre adgangskoden ved næste **logon** og dele den nye adgangskode med brugeren.

3. Det lokale Active Directory User-objekt er ikke konfigureret **korrekt** til objektsynkronisering eller synkronisering af adgangskoder. Hvis du vil foretage fejlfinding af dette problem, skal du følge de trin, der er beskrevet i [Fejlfinding af synkronisering af adgangskodehash med Azure AD Connect-synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







