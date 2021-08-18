---
title: Tilbageførsel af adgangskode virker ikke
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324917"
---
# <a name="password-writeback-is-not-working"></a>Tilbageførsel af adgangskode virker ikke

**Jeg har problemer med at konfigurere tilbageførsel af adgangskode**

- Tilbageførsel af adgangskode er en premium-funktion.
- Sørg for, at du forstår licenskravene:
  - Du skal have mindst én licens tildelt i organisationen
  - **Brugere, der kun** bruger skyen – Office 365 (O365) betalt SKU eller Azure AD Basic
  - **Sky- og/eller** lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Du kan få mere at vide om licenskrav under [Licenskrav til selvbetjening for Azure AD – nulstilling af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Du har mindst én administratorkonto og én testbrugerkonto med en af de relevante licenser.
- Du skal forbinde Azure AD-Forbind til den primære domænecontroller Emulator, for at tilbageførsel af adgangskode kan fungere. Du kan konfigurere Azure AD Forbind til at bruge en primær  domænecontroller ved at højreklikke på egenskaberne for Active Directory-synkroniseringsforbindelse og derefter vælge **konfigurer katalogpartitioner.** Derfra skal du se efter **sektionen forbindelsesindstillinger for** domænecontrolleren og markere afkrydsningsfeltet med **titlen brug kun foretrukne domænecontrollere.**
    **Bemærk!** Hvis den foretrukne DC ikke er en PDC-emulator, vil Azure AD Forbind stadig tage kontakt til PDC for at få tilbageførsel af adgangskode.
- Nulstilling af adgangskode er blevet konfigureret og aktiveret i din lejer. Du kan få mere at vide [under Giv brugerne mulighed for at nulstille deres Azure AD-adgangskoder.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Sørg for, at den administratorkonto, der bruges til at aktivere tilbageførsel af adgangskode, er en administratorkonto i skyen (oprettet i Azure AD ikke lokalt AD)
- Du har en lokal eller flerskovs-AD-installation, der kører Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2, hvor de nyeste servicepakker er installeret
- Du har Azure AD Forbind-værktøjet installeret, og du har forberedt dit AD-miljø til synkronisering med skyen. Før du tester tilbageførsel af adgangskode, skal du først fuldføre en fuld import og fuld synkronisering fra både AD og Azure AD i Azure AD Forbind.
- Du kan få mere at vide ved at se, hvordan [du kan udføre en fuld synkronisering og fuld import i Azure AD Forbind](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Jeg har et problem med forbindelse til tilbageførsel af adgangskode**

1. Download og aktivér den nyeste version [af Azure AD Forbind](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallkonfiguration: Azure AD Forbind (1.1.443 og derover) skal have **udgående HTTPS-adgang** for at:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Tillad, at inaktive forbindelser bevares i mindst 2-3 minutter

**Jeg har stadig problemer med tilbageførsel af adgangskode**

- Hvis du stadig har problemer, kan du prøve at deaktivere og genaktivere tjenesten til tilbageførsel af adgangskode i Azure AD Forbind værktøjet
- Du kan få mere at vide ved at [se, hvordan du deaktiverer og genaktiverer tilbageførsel af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
