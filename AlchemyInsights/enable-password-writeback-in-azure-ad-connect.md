---
title: Aktivér tilbageførsel af adgangskode i Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093349"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktivér tilbageførsel af adgangskode i Azure AD Connect

Hvis du vil aktivere selvbetjening til nulstilling af adgangskode, skal du først aktivere indstillingen tilbageførsel i Azure AD Connect. Fra azure AD Connect-serveren skal du udføre følgende trin:

1. Log på din Azure AD Connect-server, og start **konfigurationsguiden til Azure AD Connect.**
2. Klik på **Konfigurer** på **velkomstsiden.**
3. Vælg Tilpas **synkroniseringsindstillinger** på siden Yderligere **opgaver,** og klik derefter på **Næste.**
4. På siden **Opret forbindelse til Azure AD** skal du angive en global administratorlegitimationsoplysninger for din Azure-lejer og derefter klikke på **Næste.**
5. Klik på **Næste på filtreringssiderne** Forbind mapper og **Domæne/OU.**
6. På siden **Valgfrie funktioner** skal du markere feltet ud for tilbageførsel **af adgangskode og** klikke på **Næste.**
7. Klik på **Konfigurer på siden** Klar til konfiguration, **og** vent på, at processen afsluttes.
8. Klik på Afslut, når konfigurationen **er færdig.**

Med tilbageførsel af adgangskode aktiveret i Azure AD Connect skal du konfigurere Azure AD SSPR til tilbageførsel.  Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:

1. Log på Azure-portalen med en global administratorkonto.
2. Søg efter og vælg **Azure Active Directory,** klik på **Nulstil adgangskode,** og **klik derefter på integration i det lokale miljø.**
3. Angiv indstillingen for **Tilbageskrivning af adgangskoder til dit lokale katalog?** til **Ja.**
4. Angiv indstillingen for Tillad **brugere at låse konti op uden at nulstille deres adgangskode?** til **Ja.**
5. Klik på Gem, når du **er klar.**

Du kan finde flere oplysninger [i Aktivere tilbageførsel af adgangskode til](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)Azure Active Directory til selvbetjening til nulstilling af adgangskode i et lokalt miljø.

> [!NOTE]
>  Når en administrator nulstiller en brugers adgangskode i Azure-portalen, og den pågældende bruger er synkroniseret med organisationsnetværket eller adgangskodehash, skrives adgangskoden tilbage til det lokale miljø. Denne funktionalitet kræver Azure Premium-licens (P1 eller P2) og understøttes i øjeblikket ikke i Office-administrationsportalen.
