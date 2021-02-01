---
title: Problemer med legitimationsoplysninger
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063600"
---
# <a name="issues-with-credentials"></a>Problemer med legitimationsoplysninger

Microsoft-identitetsplatformen og flowet til klientlegitimationsoplysninger for [OAuth 2.0-klienten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beskriver, hvordan du programmerer direkte mod tildelingsflowet for OAuth 2.0-klientlegitimationsoplysninger.

**Hvordan administrerer jeg et programs adgangskode eller legitimationsoplysninger til certifikater?**

I Azure CLI kan du bruge [az ad app-legitimationsoplysninger](https://docs.microsoft.com/cli/azure/ad/app/credential) til at slette, angive eller nulstille et apps adgangskode- eller certifikatlegitimationsoplysninger.

**Hvordan nulstiller mine brugere deres adgangskoder?**

Brugerne skal registrere [sig til selvbetjening for nulstilling af adgangskode,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) før de kan nulstille deres adgangskoder. Når en bruger er registreret, kan brugeren følge instruktionerne i denne artikel for at nulstille sin adgangskode: [Nulstil din arbejds- eller skoleadgangskode.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hvordan ændrer mine brugere deres adgangskoder?**

Brugerne kan følge trinnene i denne artikel for at ændre deres adgangskoder: [Sådan ændrer du din adgangskode.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
De kan også [administrere appadgangskoder for totrinsbekræftelse.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Min bruger får en fejl, når han eller hun ændrer eller nulstiller sin adgangskode**

Dette link indeholder oplysninger om almindelige problemer, der kan opstå, når en bruger forsøger at nulstille sin adgangskode: [almindelige problemer og deres løsninger](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Jeg har problemer med at nulstille en brugers adgangskode**

- Sørg for, at du har tilladelse til at nulstille adgangskoder. *Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.* Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

- Sørg for, at du forstår licenskravene:

  - Du skal have mindst én licens tildelt i organisationen:
    - **Kun brugere i skyen** – Alle Office 365 (O365) betalte SKU'er eller Azure AD Basic
    - **Sky- og/eller** lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Du kan få mere at vide om licenskrav under Licenskrav til nulstilling af adgangskode [til Azure AD via selvbetjening.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Hvis du vil nulstille en brugers adgangskode, skal du finde brugeren i Azure AD. Klik derefter på knappen "Nulstil adgangskode" på oversigtsbladet for den pågældende bruger.

**Knappen til nulstilling af adgangskode er nedtonet**

Du er ikke autoriseret til **at nulstille** denne brugers adgangskoder. *Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.* Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se bladet til nulstilling af adgangskode**

Du er ikke autoriseret til at nulstille adgangskoder. *Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.* Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se integrations bladet i det lokale miljø ved nulstilling af adgangskode**

- Integrations bladet i det lokale miljø vises kun i hybridmiljøer – dvs. at du bruger tilbageførsel af adgangskode til at manipulere lokale brugeres adgangskoder.

- Du kan ikke se denne blade, hvis:

  - Du bruger ikke tilbageførsel af adgangskode
  - Der er et problem med din installation/forbindelse til tilbageførsel af adgangskode
  - Der er et problem med din installation/forbindelse til Azure AD Connect
  - Du kan finde flere fejlfindingstrin til problemer med tilbageførsel af adgangskode under [Fejlfinding af tilbageførsel af adgangskode](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Jeg ved ikke, hvordan jeg nulstiller en brugers adgangskode**

1. Log på Azure-portalen som en relevant administrator.
2. Gå til siden **Brugere og grupper,** og vælg **Alle brugere.**
3. Vælg en bruger på listen.
4. Vælg Oversigt for den valgte **bruger,** og vælg derefter Nulstil adgangskode på **kommandolinjen.**
5. Vælg knappen **Nulstil** adgangskode, og følg vejledningen på skærmen.
    - Kun nulstillinger, der udføres via **Azure-portalen, understøtter** tilbageførsel af adgangskode.

**Jeg nulstiller en lokal brugers adgangskode fra Office 365-administrationsportalen eller Office 365-mobilprogrammet, men brugeren kan stadig ikke logge på**

Tilbageførsel af adgangskode understøttes ikke i denne portal. Nulstil brugerens adgangskode igen i Azure-portalen.
