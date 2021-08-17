---
title: Fejlfinding af SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038952"
---
# <a name="troubleshoot-sspr"></a>Fejlfinding af SSPR

**Jeg har problemer med at konfigurere nulstilling af adgangskode**

- Hvis du er administrator og leder efter, hvordan du aktiverer selvbetjening til nulstilling af adgangskode, skal du se Selvstudium aktivere [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)for at konfigurere nulstilling af adgangskode for organisationen. Det kan også være en ide at gennemgå [licenskravene.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Du skal have mindst én licens tildelt i organisationen.
    - **Brugere, der kun** bruger skyen – Office 365 (O365) betalt SKU eller Azure AD Basic
    - **Sky- og/eller** lokale brugere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
- Hvis du har flere spørgsmål om nulstilling af adgangskode via selvbetjening, kan du se [vores ofte stillede spørgsmål.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg får en fejlmeddelelse**

Gennemse denne artikel for at finde almindelige fejl og deres løsninger: Fejlfinding i forbindelse med [nulstilling af adgangskode via selvbetjening](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg har problemer med min politik for nulstilling af adgangskode**

- Hvis din politik for nulstilling af adgangskode ikke opfører sig som forventet, eller hvis du har spørgsmål om politikker for nulstilling af adgangskode, skal du læse denne artikel: Adgangskodepolitikker og begrænsninger [i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Politikker for nulstilling af adgangskoder gælder ikke for administratorer. Microsoft gennemtvinger en stærk standardpolitik for nulstilling af adgangskode til to porte for enhver Azure-administratorrolle. Sørg for, at du tester med en bruger, der ikke er administrator. Du kan finde flere oplysninger om administratorens nulstillingspolitik i denne artikel: Forskelle [på politikker for nulstilling af administrator.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Jeg ønsker ikke, at mine brugere skal registrere yderligere sikkerhedsoplysninger til nulstilling af adgangskode**

Du kan forud udfylde data (mail og telefonattributter) for dine brugere ved hjælp af en API, PowerShell eller Azure AD Forbind. For at få mere at vide om, hvordan du læser:

- [Installation af nulstilling af adgangskode uden krav om, at brugerne skal registrere sig](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Hvilke data bruges ved nulstilling af adgangskode](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Jeg ønsker, at mine brugere skal registrere deres yderligere sikkerhedsoplysninger til nulstilling af adgangskode**

1. Få brugerne til at registrere deres sikkerhedsoplysninger til nulstilling af adgangskode ved at få dem til at [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Når dataene er udfyldt for brugeren (af brugeren eller af administratoren), skal du dirigere brugeren til [aka.ms/sspr](https://passwordreset.microsoftonline.com/) så brugerne kan få mulighed for at nulstille deres egne adgangskoder.
1. Hvis brugerne stadig oplever problemer,  er de højst sandsynligt brugere, der er medlem af organisationsnetværk eller **adgangskodehash.** Det betyder, at der sandsynligvis er et problem med tjenesten Tilbageførsel af adgangskode.