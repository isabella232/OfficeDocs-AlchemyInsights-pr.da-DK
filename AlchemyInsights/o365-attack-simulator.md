---
title: 2681 angreb simulator i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305326"
---
# <a name="attack-simulator-in-office-365"></a>Angrebs simulator i Office 365

- Er du mangler angreb Simulator? Angrebs simulator kræver **office 365 Advanced Threat Protection plan 2 (ATP plan 2)** eller **Office 365 Enterprise E5**. Angrebs Simulator er **ikke** inkluderet i Office 365 Advanced Threat Protection plan 1 (ATP plan 1), Office 365 Enterprise E3 eller et Office 365 Business-abonnement.

- Den konto, du bruger til at starte simulerede angreb, kræver global administrator-eller sikkerhedsadministrator tilladelser og multifaktorgodkendelse (MFA). Du finder flere oplysninger om angrebs simulator krav i [dette emne](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Vigtige ting at vide om **Brute Force password** angreb simuleringer:

  - Hvis der er aktiveret MFA på målkontoen, og adgangskoden blev gættet korrekt, vil kontoen ikke blive vist som kompromitteret (den anden godkendelses faktor vil være ufuldstændig).

  - Adgangskodefilen må ikke være større end 10 MB. Brug én adgangskode pr. linje, og Medtag en tom linje (vognretur) efter den sidste adgangskode på listen.

- Vigtige ting at vide om **Spear phishing** vedhæfte simuleringer:

  - Ved design kan du ikke angive en brugerdefineret værdi for **phishing-logonserverens webadresse**.

  - Hvis en modtager bruger funktionen [Aktivér rapport meddelelsen](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til at rapportere meddelelsen som phishing, modtager du muligvis ikke påmindelser om meddelelsen (fordi dette er et simuleret angreb).

- Rapporter: når det simulerede angreb er fuldført, kan du klikke på **angrebs detaljer** for at se rapporten.

- For detaljerede instruktioner og nye funktioner i Attack simulator, se [Attack simulator i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
