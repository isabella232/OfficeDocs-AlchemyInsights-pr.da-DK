---
title: 2681 Attack– –– – Microsoft 365
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
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325065"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angrebs in-Microsoft 365

- Går du glip af Angrebs problem? Attack Defender kræver **Microsoft Defender til Office 365 Plan 2** eller Office 365 Enterprise **E5.** Attack Defender er **ikke** inkluderet i Microsoft Defender Office 365 Plan 1, Office 365 Enterprise E3 eller nogen Microsoft 365 Apps for business abonnementer.

- Den konto, du bruger til at starte simulerede angreb, kræver globale administrator- eller sikkerhedsadministratortilladelser og multifaktorgodkendelse. Du kan finde flere oplysninger om krav til angrebsspil i [dette emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Vigtige ting at vide om **Brute Force-angrebssimulering** af adgangskoder:

  - Hvis målkontoen har MFA aktiveret, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelsesfaktor vil være ufuldstændig).

  - Adgangskodefilen må ikke være større end 10 MB. Brug én adgangskode pr. linje, og medtag en tom linje (vognretur) efter den sidste adgangskode på listen.

- Vigtige ting, du skal vide om **phishing-phishing, som** vedhæfter simulering:

  - Du kan ikke angive en brugerdefineret værdi for URL-adresse til **phishing-loginserver.**

  - Hvis en modtager [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) bruger tilføjelsesprogrammet Aktivér rapportmeddelelse for at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (da dette er et simuleret angreb).

- Rapporter: Når de simulerede angreb er udført, kan du klikke **på Oplysninger om angreb** for at få vist rapporten.

- Du kan finde detaljerede instruktioner og nye funktioner i Angrebs analyse [under Angrebs muligheder Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
