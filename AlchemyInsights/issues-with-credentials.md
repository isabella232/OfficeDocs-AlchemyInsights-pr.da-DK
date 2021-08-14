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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986813"
---
# <a name="issues-with-credentials"></a>Problemer med legitimationsoplysninger

Microsoft-identitetsplatform og flowet til klientlegitimationsoplysninger for [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beskriver, hvordan du programmerer direkte mod OAuth 2.0-klientlegitimationsoplysninger-flow.

**Hvordan administrerer jeg et programs adgangskode eller legitimationsoplysninger til certifikater?**

I Azure CLI kan du bruge [az ad app-legitimationsoplysninger](https://docs.microsoft.com/cli/azure/ad/app/credential) til at slette, angive eller nulstille et apps adgangskode- eller certifikatlegitimationsoplysninger.

**Hvordan nulstiller mine brugere deres adgangskoder?**

Brugerne skal tilmelde [sig nulstilling af adgangskode via selvbetjening,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) før de kan nulstille deres adgangskoder. Når en bruger er registreret, kan brugeren følge instruktionerne i denne artikel for at nulstille sin adgangskode: [Nulstil din arbejds- eller skoleadgangskode.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Hvordan ændrer mine brugere deres adgangskoder?**

Brugerne kan følge trinnene i denne artikel for at ændre deres adgangskoder: [Sådan ændrer du din adgangskode.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
De kan også [Administrere appadgangskoder for totrinsbekræftelse](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Min bruger får en fejl, når han eller hun ændrer eller nulstiller sin adgangskode**

Dette link indeholder oplysninger om almindelige problemer, der kan opstå, når en bruger forsøger at nulstille sin adgangskode: [Almindelige problemer og deres løsninger](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Jeg har problemer med at nulstille en brugers adgangskode**

- Sørg for, at du har tilladelse til at nulstille adgangskoder. *Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.* Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

- Sørg for, at du forstår licenskravene:

  - Du skal have mindst én licens tildelt i organisationen:
    - **Brugere, der kun** bruger skyen – Office 365 (O365) betalt SKU eller Azure AD Basic
    - **Sky- og/eller** lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Hvis du vil have mere at vide om licenskrav, [skal du se Licenskrav til nulstilling af](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)adgangskode til Azure AD via selvbetjening.
- Hvis du vil nulstille en brugers adgangskode, skal du finde brugeren i Azure AD. Klik derefter på knappen "nulstil adgangskode" i oversigtsruden for den pågældende bruger.

**Knappen til nulstilling af adgangskode er nedtonet**

Du er ikke autoriseret til **at nulstille** denne brugers adgangskoder. *Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.* Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se bladet til nulstilling af adgangskode**

Du er ikke autoriseret til at nulstille adgangskoder. *Kun globale administratorer, adgangskoder og brugeradministratorer kan nulstille brugeradgangskoder.* Globale administratorer kan også nulstille andre privilegerede administratorers adgangskoder.

**Jeg kan ikke se integrations bladet i det lokale miljø ved nulstilling af adgangskode**

- Integrations bladet i det lokale miljø vises kun i hybridmiljøer – hvilket betyder, at du bruger tilbageførsel af adgangskode til at manipulere brugernes adgangskoder i det lokale miljø.

- Du kan ikke se dette blad, hvis:

  - Du bruger ikke tilbageførsel af adgangskode
  - Der er et problem med din installation/forbindelse til tilbageførsel af adgangskode
  - Der er et problem med din installation/forbindelse til Azure AD Forbind
  - Du kan finde flere fejlfindingstrin til problemer med tilbageførsel af adgangskode i [Fejlfinding af tilbageførsel af adgangskode](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Jeg ved ikke, hvordan jeg nulstiller en brugers adgangskode**

1. Log på Azure-portalen som en passende administrator.
2. Gå til **bladet Brugere og** grupper, og vælg Alle **brugere**.
3. Vælg en bruger på listen.
4. For den valgte bruger skal du **vælge Oversigt**, og derefter skal du på kommandolinjen vælge **Nulstil adgangskode**.
5. Vælg knappen **Nulstil** adgangskode, og følg vejledningen på skærmen.
    - Kun nulstillinger, der udføres via **Azure-portalen, understøtter** tilbageførsel af adgangskode.

**Jeg nulstiller en brugers adgangskode i det lokale miljø fra Office 365 Admin-portalen eller Office 365-mobilprogrammet, men brugeren kan stadig ikke logge på**

Tilbageførsel af adgangskode understøttes ikke i denne portal. Nulstil brugerens adgangskode igen i Azure-portalen.
