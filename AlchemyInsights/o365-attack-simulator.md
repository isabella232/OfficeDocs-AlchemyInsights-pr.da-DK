---
title: 2681 Angreb Simulator i Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506732"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angreb Simulator i Microsoft 365

- Er du mangler Angreb Simulator? Angrebssimulator kræver **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** eller **Office 365 Enterprise E5**. Attack Simulator er **ikke** inkluderet i Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 eller microsoft 365 Apps til virksomheder-abonnementer.

- Den konto, du bruger til at starte simulerede angreb, kræver globale administrator- eller sikkerhedsadministratortilladelser og MFA (multifaktorgodkendelse). Yderligere oplysninger om krav til angrebssimulator finder du i [dette emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Vigtige ting at vide om **Brute Force Password** angreb simuleringer:

  - Hvis målkontoen har aktiveret MFA, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelsesfaktor vil være ufuldstændig).

  - Adgangskodefilen må ikke være større end 10 MB. Brug én adgangskode pr. linje, og medtag en tom linje (vognretur) efter den sidste adgangskode på listen.

- Vigtige ting at vide om **Spear Phishing** vedhæfte simuleringer:

  - Efter design kan du ikke angive en brugerdefineret værdi for **URL-adressen til phishing-loginserveren**.

  - Hvis en modtager bruger [tilføjelsesprogrammet Aktivér rapportmeddelelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (fordi dette er et simuleret angreb).

- Rapporter: Når det simulerede angreb er fuldført, kan du klikke på **Angrebsoplysninger** for at se rapporten.

- Yderligere oplysninger og nye funktioner i Attack Simulator finder du i [Attack Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
