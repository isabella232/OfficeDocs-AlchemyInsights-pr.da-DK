---
title: Problem med nulstilling af adgangskode
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039960"
---
# <a name="problems-resetting-password"></a>Problemer med nulstilling af adgangskode

Følgende er nogle af de problemer, du kan komme ud for, når du nulstiller adgangskode og de mulige løsninger:

**Jeg har et problem med nulstilling af adgangskode, der ikke er dækket af de andre kategorier**

- Sørg for, at du har tilladelse til at nulstille adgangskoder. Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder. Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.
- Sørg for, at du forstår licenskravene:
    - Du skal have mindst én licens tildelt i organisationen
        - Brugere, der kun bruger skyen – Office 365 (O365) betalt SKU eller Azure AD Basic
        - Sky- og/eller lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
        - Du kan læse mere om licenskrav i artiklen [Licenskrav til selvbetjening for Azure AD – nulstilling af adgangskode.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg har problemer med at teste den politik for nulstilling af adgangskode, jeg har angivet**

- For nylig anvendte politikker kan det tage flere minutter at replikere på tværs af alle datacentre og slutpunkter. Fysisk afstand fra datacenteret påvirker også, hvor hurtigt ændringerne anvendes.
- Test med en slutbruger, ikke en administrator, og test med et lille sæt af brugere. De politikker, der er konfigureret i Azure-portalen, gælder KUN for slutbrugere, ikke administratorer. Microsoft gennemtvinger en stærk standardpolitik for nulstilling af adgangskode til to porte for alle Azure-administratorroller (Eksempel: Global administrator, Helpdesk-administrator, Adgangskodeadministrator osv.)
    - Få mere at vide [om politikker for administratorer](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Jeg vil installere nulstilling af adgangskode, men jeg vil ikke have mine brugere til at registrere yderligere sikkerhedsoplysninger**

Forudindstille data for dine brugere, så de ikke behøver at gøre det! – Som administrator kan du angive telefon- og mailegenskaber for dine brugere, før du udruller nulstilling af adgangskode til organisationen. Du kan gøre dette ved hjælp af en API, PowerShell eller Azure AD Forbind. Flere oplysninger her:
- [Installation af nulstilling af adgangskode uden krav om, at brugerne skal registrere sig](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Hvilke data bruges ved nulstilling af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Knappen til nulstilling af adgangskode er nedtonet**

Du er ikke autoriseret til at nulstille denne brugers adgangskoder. Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder. Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se bladet til nulstilling af adgangskode**

Du er ikke autoriseret til at nulstille adgangskoder. Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder. Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se integrations bladet i det lokale miljø ved nulstilling af adgangskode**

- Integrations bladet i det lokale miljø vises kun i hybridmiljøer – hvilket betyder, at du bruger tilbageførsel af adgangskode til at manipulere brugernes adgangskoder i det lokale miljø.
- Du kan ikke se dette blad, hvis:
    - Du bruger ikke tilbageførsel af adgangskode
    - Der er et problem med din installation/forbindelse til tilbageførsel af adgangskode
    - Der er et problem med din installation/forbindelse til Azure AD Forbind
    - Du kan finde flere fejlfindingstrin til problemer med tilbageførsel af adgangskode i afsnittet Fejlfinding af [tilbageførsel af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg ved ikke, hvordan jeg nulstiller en brugers adgangskode**

1. Log på Azure-portalen som en passende administrator.
1. Gå til bladet Brugere og grupper, og vælg **Alle brugere**.
1. Vælg en bruger på listen.
1. For den valgte bruger skal du **vælge Oversigt** og derefter klikke på Nulstil adgangskode på **kommandolinjen**.
1. Følg vejledningen på skærmen.
    - Kun nulstillinger, der udføres via Azure-portalen, understøtter tilbageførsel af adgangskode.

**Jeg nulstiller en brugers adgangskode i det lokale miljø fra Office 365 Admin-portalen eller Office 365-mobilprogrammet, men brugeren kan stadig ikke logge på**

Tilbageførsel af adgangskode understøttes ikke i denne portal. Nulstil brugerens adgangskode igen i Azure-portalen – portal.azure.com

