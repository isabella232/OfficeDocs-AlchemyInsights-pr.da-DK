---
title: Automatisk klassificering opfører sig ikke som forventet med AIP-klienten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820892"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatisk klassificering opfører sig ikke som forventet med AIP-klienten

Automatisk klassificering opfører sig ikke som forventet. Brug følgende anbefalede retningslinjer:

1. Hvis du har problemer med automatisk mærkning, skal du se Sådan konfigurerer du betingelser for automatisk og anbefalet klassificering [af Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og Hvad typerne af følsomme oplysninger søger [efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Kontrollér, om du bruger omfangsspecifikke politikker, der ikke er konfigureret korrekt: Sådan konfigureres politikken for Azure Information Protection for bestemte brugere ved hjælp af politikker med [omfang.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Hvis automatisk mærkning ikke fungerer i Outlook, når du vedhæfter et mærket dokument, skal du kontrollere, at dette ikke er defineret som beskrevet `DRMEncryptProperty` her: IRM-indstillinger for sikkerhed [i registreringsdatabasen.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Hvis du har brugt de [indbyggede oplysningstyper til din](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) Azure Information Protection-politik, skal du kontrollere, at indholdet svarer til det forventede format.
5. Kontrollér, at etiketten er korrekt konfigureret til **Automatisk** eller **Anbefalet.** (**Automatisk** mærkning er tilgængelig for alle Microsoft  365-apps, hvorimod Anbefalet er tilgængelig for alle Microsoft 365-apps med undtagelse af Outlook.)
6. Du kan ikke bruge automatisk klassificering af dokumenter og mails, der tidligere var manuelt mærket eller tidligere automatisk mærket med en højere klassificering.  Du kan finde flere oplysninger i: [Sådan anvendes automatiske eller anbefalede etiketter.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Hvis du stadig oplever problemer, skal du indsamle Azure Information Protection-klientlogfiler og vedhæfte de eksporterede logfiler til din supportbillet. Sådan eksporterer du Azure Information Protection-logfiler:
    - Åbn et Office-dokument, eller opret en ny mail i Outlook.
    - Klik **på Beskyt/følsomhed**  >  **hjælp og feedback**.
    - Klik **på Eksportér logfiler.**
    - Gem logfilerne til det sted, du vil gemme dem, og vedhæft dem til din serviceanmodning.

Du kan finde flere oplysninger i:

- [Sådan konfigurerer du betingelser for automatisk og anbefalet klassificering af Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Vejledninger til almindelige scenarier, der bruger Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Gennemse Azure Information Protection-dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Gennemse Azure Information Protection-abonnementer og -funktioner](https://azure.microsoft.com/pricing/details/information-protection)
- [Krav til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Quick Start-selvstudium til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Download Azure Information Protection-klienten](https://www.microsoft.com/download/details.aspx?id=53018)
