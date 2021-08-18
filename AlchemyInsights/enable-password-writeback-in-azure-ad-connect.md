---
title: Aktivér tilbageførsel af adgangskode i Azure AD-Forbind
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118198"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktivér tilbageførsel af adgangskode i Azure AD-Forbind

Hvis du vil aktivere selvbetjening til nulstilling af adgangskode, skal du først aktivere indstillingen tilbageførsel i Azure AD Forbind. Fra Azure AD Forbind skal du udføre følgende trin:

1. Log på Din Azure AD Forbind-server, og start **guiden til konfiguration Forbind Azure AD.**
2. På siden **Velkommen skal** du klikke på **Konfigurer.**
3. På siden **Yderligere opgaver skal** du vælge Tilpas **synkroniseringsindstillinger** og derefter klikke på **Næste.**
4. På siden **Forbind til Azure AD** skal du angive en global administratoroplysninger for din Azure-lejer og derefter klikke på **Næste.**
5. På siden Forbind og **Domæne/OU-filtreringssider** skal du klikke på **Næste.** 
6. På siden **Valgfrie funktioner** skal du markere afkrydsningsfeltet ud for **Tilbageførsel af adgangskode og** klikke på **Næste.**
7. Klik på **Konfigurer på siden** Klar til konfiguration, og vent på, at processen afsluttes. 
8. Når du ser konfigurationen færdig, skal du klikke på **Afslut.**

Med tilbageførsel af adgangskode aktiveret i Azure AD Forbind du konfigurere Azure AD SSPR til tilbageførsel.  Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:

1. Log på Azure-portalen med en global administratorkonto.
2. Søg efter og vælg **Azure Active Directory**, klik **på Nulstil adgangskode**, og klik derefter på Integration i det lokale **miljø**.
3. Angiv indstillingen for **Tilbageskrivning af adgangskoder til din lokale mappe?** til **Ja.**
4. Angiv indstillingen tillad brugere **at låse konti op uden at nulstille deres adgangskode?** til **Ja.**
5. Når du er klar, skal du klikke **på Gem**.

Du kan finde flere oplysninger Azure Active Directory Aktivér selvbetjening [for nulstilling af adgangskode i et lokalt miljø.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)

> [!NOTE]
>  Når en administrator nulstiller en brugers adgangskode i Azure-portalen, og den pågældende bruger er organisationsnetværks- eller adgangskodehash synkroniseret, skrives adgangskoden tilbage til det lokale miljø. Denne funktion kræver Azure Premium-licens (P1 eller P2) og understøttes i øjeblikket ikke i Office Administration.
