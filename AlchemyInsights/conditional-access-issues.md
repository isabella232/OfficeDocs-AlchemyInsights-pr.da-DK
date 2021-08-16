---
title: Problemer med betinget adgang
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069958"
---
# <a name="conditional-access-issues"></a>Problemer med betinget adgang

**Løs problemer med Logondiagnosticering**

Du kan hurtigt finde ud af, hvad der skete, eller diagnosticere problemer i forbindelse med brugerlogføring ved hjælp af [Log på-diagnosticering:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Start Logondiagnosticering.
1. Find hændelsen, der skal analyseres, ved at angive i de oplysninger, du har om brugeren, programmet, tidspunktet for logon, anmodnings-id eller korrelations-id.
1. Gennemgå de diagnostiske resultater, der viser, hvad der er sket, og hvilke handlinger du kan udføre for at foretage ændringer (hvis der er behov for ændringer).

**Trin til fejlfinding af et logon** 

1. Gå til Azure AD-logonsiden.
1. Filtrer logons efter bruger, tidsinterval, program, status, klientapp osv.
1. Vælg en logonhændelse, og få vist fanen Betinget adgang for at se, hvilke politikker der blev evalueret.
1. Klik på rækken i en politik for at få vist politikdetaljerne og forstå, hvorfor den er anvendt.

**Værktøjer til fejlfinding af en politik for betinget adgang**

- Rapporttilstand giver dig mulighed for at evaluere en politik uden at påvirke brugere.
- Med what if-værktøjet kan du simulere logonhændelser og se, hvilke politikker der gælder.
- Insights projektmappe i realtid viser indvirkningen af hver politik i realtid.

**Politikker for beskyttelse af oprindelige planer**

Politikker for oprindelig beskyttelse frarådes. De gennemtvinges ikke længere og fjernes snart fra Azure-portalen. Vi anbefaler, at [du aktiverer sikkerhedsstandardindstillinger.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Du kan finde flere oplysninger om Betinget adgang i:

[Bedste fremgangsmåder for betinget adgang i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Betingelser i Betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrolelementer i Betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Placeringer i Betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
