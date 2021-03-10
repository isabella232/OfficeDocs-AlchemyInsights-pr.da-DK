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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693390"
---
# <a name="problems-resetting-password"></a>Problemer med nulstilling af adgangskode

Følgende er nogle af de problemer, du kan komme ud for, når du nulstiller adgangskoden og de mulige løsninger:

**Jeg har et problem med nulstilling af adgangskode, der ikke er dækket af de andre kategorier**

- Sørg for, at du er godkendt til at nulstille adgangskoder. Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder. Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.
- Sørg for, at du forstår licenskravene:
    - Du skal have mindst én licens tildelt i organisationen
        - Kun brugere i skyen – Alle Office 365 (O365) betalte SKU'er eller Azure AD Basic
        - Sky- og/eller lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
        - Du kan læse mere om licenskrav i artiklen [Licenseringskrav til nulstilling](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)af adgangskode til Azure AD via selvbetjening.

**Jeg har problemer med at teste den politik for nulstilling af adgangskode, jeg har angivet**

- De senest anvendte politikker kan tage flere minutter at replikere på tværs af alle datacentre og slutpunkter. Fysisk afstand fra datacenteret påvirker også, hvor hurtigt ændringerne anvendes.
- Test med en slutbruger, ikke en administrator, og test med et lille sæt af brugere. De politikker, der er konfigureret i Azure-portalen, gælder KUN for slutbrugere, ikke administratorer. Microsoft har en stærk standardpolitik for nulstilling af adgangskode til to porte for alle Azure-administratorroller (eksempel: Global administrator, Helpdesk-administrator, Adgangskodeadministrator osv.)
    - Få mere at vide [om politikker for administratorer.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Jeg vil installere nulstilling af adgangskode, men jeg vil ikke have mine brugere til at registrere yderligere sikkerhedsoplysninger**

Forudindstille data for dine brugere, så de ikke behøver at gøre det! – Som administrator kan du angive telefon- og mailegenskaber for dine brugere, før du udruller nulstilling af adgangskode til organisationen. Du kan gøre dette ved hjælp af en API, PowerShell eller Azure AD Connect. Flere oplysninger her:
- [Installation af nulstilling af adgangskode uden at kræve, at brugerne skal registrere sig](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Hvilke data bruges ved nulstilling af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Knappen til nulstilling af adgangskode er nedtonet**

Du er ikke autoriseret til at nulstille denne brugers adgangskoder. Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder. Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se bladet til nulstilling af adgangskode**

Du er ikke autoriseret til at nulstille adgangskoder. Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder. Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se integrations bladet i det lokale miljø ved nulstilling af adgangskode**

- Integrations bladet i det lokale miljø vises kun i hybridmiljøer – dvs. at du bruger tilbageførsel af adgangskode til at manipulere lokale brugeres adgangskoder.
- Du kan ikke se denne blade, hvis:
    - Du bruger ikke tilbageførsel af adgangskode
    - Der er et problem med din installation/forbindelse til tilbageførsel af adgangskode
    - Der er et problem med din installation/forbindelse til Azure AD Connect
    - Du kan finde flere fejlfindingstrin til problemer med tilbageførsel af adgangskode i afsnittet Fejlfinding [af tilbageskrivning af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg ved ikke, hvordan jeg nulstiller en brugers adgangskode**

1. Log på Azure-portalen som en relevant administrator.
1. Gå til siden Brugere og grupper, og vælg **Alle brugere.**
1. Vælg en bruger på listen.
1. Vælg Oversigt for den valgte **bruger,** og klik derefter på Nulstil adgangskode på **kommandolinjen.**
1. Følg vejledningen på skærmen.
    - Kun nulstillinger, der udføres via Azure-portalen, understøtter tilbageførsel af adgangskode.

**Jeg nulstiller en lokal brugers adgangskode fra Office 365-administrationsportalen eller Office 365-mobilprogrammet, men brugeren kan stadig ikke logge på**

Tilbageførsel af adgangskode understøttes ikke i denne portal. Nulstil brugerens adgangskode igen i Azure-portalen – portal.azure.com

