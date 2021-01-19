---
title: Fejl i bruger logger
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900857"
---
# <a name="user-sign-in-errors"></a>Fejl i bruger logger

**Løse problemer med logon-diagnosticering**

Hvis du vil registrere årsagen eller diagnose problemer, der er relateret til brugerlogon, skal du udføre følgende trin:

1. Start den [diagnosticering, du har logget på](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Find den hændelse, der skal analyseres, ved at angive de oplysninger, du har om brugeren, programmet, klokkeslættet for logon, anmodnings-id eller korrelations-id.
3. Gennemgå de diagnostiske resultater, der viser oplysninger om, hvad der er sket, og hvilke handlinger du kan udføre for at foretage ændringer, hvis der er behov for ændringer.

**Leder du efter oplysninger om de AADSTS-fejlkoder, der returneres fra Azure Active Directory (Azure AD) sikkerhedstokentjenesten (STS)?** Læs [denne artikel](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) for at finde AADSTS-fejlbeskrivelser, rettelser og nogle forslag til løsninger