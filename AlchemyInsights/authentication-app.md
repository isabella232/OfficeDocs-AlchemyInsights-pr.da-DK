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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404597"
---
# <a name="authentication-app"></a>Godkendelsesapp

Hvis du er global administrator, kan du hurtigt finde ud af, hvad der skete, eller diagnosticere problemer relateret til brugerlogning ved hjælp af [Logondiagnosticering.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Start diagnosticeringen ved at klikke på knappen "[Start diagnosticering".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Find den hændelse, du vil analysere, ved at angive de oplysninger, du har om brugeren, programmet, tidspunktet for logon, anmodnings-id eller korrelations-id.
1. Gennemgå de diagnostiske resultater, der viser detaljer om, hvad der er sket, og hvilke handlinger du kan udføre for at foretage ændringer, hvis der er behov for ændringer.

**Kontrollér det scenarie, der er relevant:**

1. Hvis en bruger ikke får en pushmeddelelse i Microsoft Authenticator-appen, skal du bekræfte, at de ikke vises under de MFA-blokerede brugere som beskrevet i Bloker og fjerne [blokeringen af brugere.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Hvis brugeren ikke er blokeret for MFA, men ikke modtager en pushmeddelelse, kan brugeren åbne Microsoft Authenticator-appen, som trækker de ventende godkendelsesanmodninger.
1. Som alternativ logonmetode kan brugeren også klikke på Log på en anden måde og vælge at bruge en bekræftelseskode fra min mobilapp.
1. Microsoft Authenticator-appen er den eneste tilgængelige metode for mange brugere. [Få mere at vide om sikkerhedsstandard,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)se [Ofte stillede spørgsmål om Authenticator-appen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for ofte stillede spørgsmål, og hvordan du kan løse dem.
 
**Anbefalede videoer**

[Sådan konfigurerer du Authenticator-appen på en ny telefon (2 minutter).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
