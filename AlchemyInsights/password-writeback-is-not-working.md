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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243288"
---
# <a name="password-writeback-is-not-working"></a>Tilbageførsel af adgangskode virker ikke

**Jeg har problemer med at konfigurere tilbageførsel af adgangskode**

- Tilbageførsel af adgangskode er en premium-funktion.
- Sørg for, at du forstår licenskravene:
  - Du skal have mindst én licens tildelt i organisationen
  - **Kun brugere i skyen** – Alle Office 365 (O365) betalte SKU'er eller Azure AD Basic
  - **Sky- og/eller** lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Du kan få mere at vide om licenskrav under [Licenskrav til nulstilling](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) af adgangskode til Azure AD via selvbetjening
- Du har mindst én administratorkonto og én testbrugerkonto med en af de relevante licenser.
- Du skal oprette forbindelse mellem Azure AD Connect og Den primære domænecontroller-emulator, for at tilbageførsel af adgangskode kan fungere. Du kan konfigurere Azure AD Connect til at bruge en  primær domænecontroller ved at højreklikke på egenskaberne for Active Directory-synkroniseringsforbindelse og derefter vælge **konfigurer katalogpartitioner.** Derfra skal du kigge efter **sektionen forbindelsesindstillinger** for domænecontrolleren og markere afkrydsningsfeltet med titlen brug **kun foretrukne domænecontrollere.**
  > [!NOTE]
  > Hvis den foretrukne DC ikke er en PDC-emulator, vil Azure AD Connect stadig nå ud til PDC for at få tilbageførsel af adgangskode.
- Nulstilling af adgangskode er konfigureret og aktiveret i din lejer. Du kan finde flere oplysninger i [Aktivere brugere til at nulstille deres Azure AD-adgangskoder.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Sørg for, at den administratorkonto, der bruges til at aktivere tilbageførsel af adgangskode, er en skybaseret administratorkonto (oprettet i Azure AD ikke i det lokale AD)
- Du har en lokal enkelt- eller flerskovs-AD-installation, der kører Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de nyeste servicepakker installeret
- Du har Azure AD Connect-værktøjet installeret, og du har forberedt dit AD-miljø til synkronisering med skyen. Før du tester tilbageførsel af adgangskode, skal du først fuldføre en fuld import og fuld synkronisering fra både AD og Azure AD i Azure AD Connect.
- Du kan få mere at vide ved at se, hvordan [du kan udføre en fuld synkronisering og fuld import i Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Jeg har et problem med forbindelse til tilbageførsel af adgangskode**

1. Download og aktivér den nyeste version af [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallkonfiguration: Azure AD Connect-værktøjet (1.1.443 og derover) skal have **udgående HTTPS-adgang** for at:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Tillad, at inaktive forbindelser bevares i mindst 2-3 minutter

**Jeg har stadig problemer med tilbageførsel af adgangskode**

- Hvis du stadig har problemer, kan du prøve at deaktivere og genaktivere tjenesten til tilbageførsel af adgangskode i Azure AD Connect-værktøjet
- Du kan få mere at vide ved at [se, hvordan du deaktiverer og genaktiverer tilbageførsel af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
