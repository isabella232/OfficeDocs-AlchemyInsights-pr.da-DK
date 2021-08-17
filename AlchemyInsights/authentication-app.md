---
title: Godkendelsesapp
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082936"
---
# <a name="authentication-app"></a>Godkendelsesapp

Hvis du er global administrator, kan du hurtigt finde ud af, hvad der skete, eller diagnosticere problemer i forbindelse med brugerlogføring ved hjælp af [Logondiagnosticering.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Start diagnosticeringen ved at klikke på knappen "[Start](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)diagnosticering". 
1. Find hændelsen, der skal analyseres, ved at angive i de oplysninger, du har om brugeren, programmet, tidspunktet for logon, anmodnings-id eller korrelations-id.
1. Gennemgå de diagnostiske resultater, der viser, hvad der er sket, og hvilke handlinger du kan udføre for at foretage ændringer, hvis der er behov for ændringer.

**Kontrollér det scenarie, der er relevant:**

1. Hvis en bruger ikke får en pushmeddelelse i Microsoft Authenticator-appen, skal du kontrollere, at de ikke vises under MFA-blokerede brugere som beskrevet i Bloker og fjern blokering [af brugere.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Hvis brugeren ikke er blokeret for MFA, men ikke modtager en pushmeddelelse, kan brugeren åbne Microsoft Authenticator-appen, som trækker de ventende godkendelsesanmodninger.
1. Som en alternativ logonmetode kan brugeren også klikke på Log på på en anden måde og vælge at bruge en bekræftelseskode fra min mobilapp.
1. Appen Microsoft Authenticator er den eneste tilgængelige metode for mange brugere. [Få mere at vide om sikkerhedsstandardindstillinger,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)se [ofte Authenticator ofte](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) stillede spørgsmål i App, og hvordan du løser dem.
 
**Anbefalede videoer**

[Sådan konfigurerer du Authenticator app på en ny telefon (2 minutter).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
