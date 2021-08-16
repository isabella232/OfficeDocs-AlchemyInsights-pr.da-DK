---
title: 2681 Attack– – – Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065278"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angrebs in-Microsoft 365

- Går du glip af Angrebs problem? Attack Defender kræver **Microsoft Defender til Office 365 Plan 2** eller Office 365 Enterprise **E5.** Attack Defender er **ikke** inkluderet i Microsoft Defender Office 365 Plan 1, Office 365 Enterprise E3 eller nogen Microsoft 365 Apps for business abonnementer.

- Den konto, du bruger til at starte simulerede angreb, kræver globale administrator- eller sikkerhedsadministratortilladelser og multifaktorgodkendelse. Du kan finde flere oplysninger om krav til angrebsspil i [dette emne](/microsoft-365/security/office-365-security/attack-simulator).

- Vigtige ting at vide om **Brute Force-angrebssimulering** af adgangskoder:

  - Hvis målkontoen har MFA aktiveret, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelsesfaktor vil være ufuldstændig).

  - Adgangskodefilen må ikke være større end 10 MB. Brug én adgangskode pr. linje, og medtag en tom linje (vognretur) efter den sidste adgangskode på listen.

- Vigtige ting, du skal vide om **phishing-phishing, som** vedhæfter simulering:

  - Du kan ikke angive en brugerdefineret værdi for URL-adresse til **phishing-loginserver.**

  - Hvis en modtager [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) bruger tilføjelsesprogrammet Aktivér rapportmeddelelse for at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (da dette er et simuleret angreb).

- Rapporter: Når de simulerede angreb er udført, kan du klikke **på Oplysninger om angreb** for at få vist rapporten.

- Hvis du vil have detaljeret vejledning og nye funktioner i Angrebsangreb, skal [du se Angrebs muligheder Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
