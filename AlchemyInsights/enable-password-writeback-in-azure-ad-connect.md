---
title: Aktivere tilbageførsel af adgangskode i Azure AD Connect
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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560434"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktivere tilbageførsel af adgangskode i Azure AD Connect

Hvis du vil aktivere tilbageførsel af adgangskode for selvbetjening, skal du først aktivere indstillingen tilbageskrivning i Azure AD Connect. I Azure AD Connect-serveren skal du udføre følgende trin:

1. Log på din Azure AD Connect-server, og Start guiden **Azure ad Connect** Configuration.
2. Klik på **Konfigurer** på siden **Velkommen** .
3. Vælg **Tilpas synkroniseringsindstillinger** på siden **flere opgaver** , og klik derefter på **næste**.
4. På siden **Opret forbindelse til Azure ad** skal du angive en global administrators legitimationsoplysninger for din Azure-lejer, og derefter skal du klikke på **næste**.
5. Klik på **næste** på siden **Opret forbindelse til mapper** og **domæne/ou** -filtrering.
6. På siden **valgfrie funktioner** skal du markere afkrydsningsfeltet ud for **adgangskode tilbageførsel** og klikke på **næste**.
7. På siden **klar til at konfigurere** skal du klikke på **Konfigurer** og vente på, at processen afsluttes.
8. Når du får vist konfigurations slutdatoen, skal du klikke på **Afslut**.

Når tilbageførsel af adgangskode er aktiveret i Azure AD Connect, skal du konfigurere Azure AD SSPR for tilbageførsel.  Hvis du vil aktivere tilbageførsel af adgangskode i SSPR, skal du udføre følgende trin:

1. Log på Azure-portalen ved hjælp af en global administratorkonto.
2. Søg efter og vælg **Azure Active Directory**, klik på **nulstilling af adgangskode**, og klik derefter på **lokal integration**.
3. Angiv indstillingen for **skrivning af adgangskoder til din lokale adresseliste?** til **Ja**.
4. Angiv indstillingen for **Tillad brugere at låse konti op uden at nulstille deres adgangskode?** til **Ja**.
5. Klik på **Gem**, når du er klar.

Hvis du vil have mere at vide, skal du se [aktivere tilbageførsel af Active Directory-selvbetjenings funktionen til nulstilling af adgangskode til et lokalt miljø](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Når en administrator nulstiller en brugers adgangskode i Azure-portalen, og hvis den pågældende bruger er sammenkædet med en adgangskode, der er synkroniseret, skrives adgangskoden tilbage til det lokale miljø. Denne funktion understøttes i øjeblikket ikke i Office-administratorportalen.