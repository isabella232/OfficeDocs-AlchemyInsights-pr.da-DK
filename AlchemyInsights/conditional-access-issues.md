---
title: Betingede adgangsproblemer
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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014787"
---
# <a name="conditional-access-issues"></a>Betingede adgangsproblemer

**Løse problemer med logon-diagnosticering**

Du kan hurtigt finde ud af, hvad der skete eller diagnosticere problemer i forbindelse med brugerlogon, ved hjælp af [logonsessionen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Start den diagnosticering, du har logget på.
1. Find den hændelse, der skal analyseres, ved at angive de oplysninger, du har om bruger, program, tidspunkt for logon, anmodnings-id eller korrelations-id.
1. Gennemgå de diagnostiske resultater, der viser oplysninger om, hvad der skete, og hvilke handlinger du kan udføre for at foretage ændringer (hvis der er behov for ændringer).

**Trin til fejlfinding af et logon** 

1. Gå til siden Azure AD-logonsiden.
1. Filtrere logon-programmer efter bruger, tidsinterval, program, status, klient-app osv.
1. Vælg en logonindstilling, og få vist fanen betinget adgang for at se, hvilke politikker der blev evalueret.
1. Klik på rækken for en politik for at få vist politik detaljerne og forstå, hvorfor den er anvendt.

**Værktøjer til fejlfinding af en politik for betinget adgang**

- Med rapport baseret tilstand kan du evaluere en politik uden at påvirke brugerne.
- Hvad hvis-værktøj gør det muligt at simulere logon-begivenheder og se, hvilke politikker der gælder.
- Indsigt og rapporterings projektmapper viser realtids virkninger for hver politik.

**Grundlæggende beskyttelsespolitikker**

Grundlæggende beskyttelsespolitikker er blevet frarådet. De håndhæves ikke længere og vil snart blive fjernet fra Azure-portalen. Vi anbefaler, at du aktiverer [sikkerhedsstandarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Hvis du vil have mere at vide om betinget adgang, skal du se:

[Bedste fremgangsmåder for betinget adgang i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Betingelser i betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrolelementer i betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Placeringer i betinget adgang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
