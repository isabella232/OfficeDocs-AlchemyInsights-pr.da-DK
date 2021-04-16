---
title: Aktivér tilbageførsel af adgangskode i Azure AD Connect
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
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814006"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktivér tilbageførsel af adgangskode i Azure AD Connect

Hvis du vil aktivere selvbetjening til nulstilling af adgangskode, skal du først aktivere indstillingen tilbageførsel i Azure AD Connect. Fra Azure AD Connect-serveren skal du udføre følgende trin:

1. Log på din Azure AD Connect-server, og start **konfigurationsguiden til Azure AD Connect.**
2. På siden **Velkommen skal** du klikke på **Konfigurer.**
3. På siden **Yderligere opgaver skal** du vælge Tilpas **synkroniseringsindstillinger** og derefter klikke på **Næste.**
4. På siden **Opret forbindelse til Azure AD** skal du angive legitimationsoplysninger som global administrator for din Azure-lejer og derefter klikke på **Næste.**
5. På siderne **Forbind kataloger** **og Domæne/OU-filtrering** skal du klikke på **Næste.**
6. På siden **Valgfrie funktioner** skal du markere afkrydsningsfeltet ud for **Tilbageførsel af adgangskode og** klikke på **Næste.**
7. Klik på **Konfigurer på siden** Klar til konfiguration, og vent på, at processen afsluttes. 
8. Når du ser konfigurationen færdig, skal du klikke på **Afslut.**

Med tilbageførsel af adgangskode aktiveret i Azure AD Connect skal du konfigurere Azure AD SSPR til tilbageførsel.  Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:

1. Log på Azure-portalen med en global administratorkonto.
2. Søg efter og vælg **Azure Active Directory**, klik på **Nulstil adgangskode**, og klik derefter på Integration i det lokale **miljø**.
3. Angiv indstillingen for **Tilbageskrivning af adgangskoder til din lokale mappe?** til **Ja.**
4. Angiv indstillingen tillad brugere **at låse konti op uden at nulstille deres adgangskode?** til **Ja.**
5. Når du er klar, skal du klikke **på Gem**.

Få mere at vide under [Aktivér tilbageførsel](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)af adgangskode til nulstilling af adgangskode til Azure Active Directory i et lokalt miljø.

> [!NOTE]
>  Når en administrator nulstiller en brugers adgangskode i Azure-portalen, og den pågældende bruger er organisationsnetværks- eller adgangskodehash synkroniseret, skrives adgangskoden tilbage til det lokale miljø. Denne funktionalitet kræver Azure Premium-licens (P1 eller P2) og understøttes ikke i øjeblikket i Office-administrationsportalen.
