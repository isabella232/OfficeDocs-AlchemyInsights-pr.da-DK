---
title: 2681-angrebs simulator i Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801545"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angrebs simulator i Microsoft 365

- Mangler du angrebs Simulator? Angrebs simulatoren kræver **Microsoft Defender til Office 365-plan 2 (DTT-plan 2)** eller **Office 365 Enterprise E5** . Angrebs simulatoren er **ikke** inkluderet i Microsoft Defender til Office 365 plan 1 (DTT plan 1), Office 365 Enterprise E3 eller eventuelle Microsoft 365-apps til virksomheds abonnementer.

- Den konto, du bruger til at køre simulerede angreb, kræver globale administrator-eller sikkerhedsadministrator tilladelser og multifaktorgodkendelse (MFA). Hvis du vil have mere at vide om krav til angrebs simulator, skal du se [dette emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Vigtige ting, du skal vide om **Brute Gennemtving** simulerede adgangskode angreb:

  - Hvis destinationskontoen er MFA aktiveret, og adgangskoden blev gættet korrekt, vises kontoen ikke som kompromitteret (den anden godkendelses faktor er ufuldstændig).

  - Adgangskodefilen må ikke være større end 10 MB. Brug én adgangskode pr. linje, og Medtag en tom linje (vognretur) efter den sidste adgangskode på listen.

- Vigtige ting, du skal vide om **Spear phishing** -tilkoblings simuleringer:

  - Du kan ikke angive en brugerdefineret værdi til **URL-adressen til phishing-logonserveren** .

  - Hvis en modtager bruger funktionen [Aktivér tilføjelse af rapport meddelelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til at rapportere meddelelsen som phishing, modtager du muligvis ikke beskeder om meddelelsen (fordi dette er et simuleret angreb).

- Rapporter: når det simulerede angreb er fuldført, kan du klikke på **oplysninger om angreb** for at få vist rapporten.

- Du kan få mere at vide om de nye funktioner i angrebs simulatoren under [angrebs simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
