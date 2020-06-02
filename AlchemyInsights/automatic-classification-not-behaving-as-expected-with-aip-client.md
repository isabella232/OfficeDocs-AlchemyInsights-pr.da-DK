---
title: Automatisk klassificering, der ikke fungerer som forventet med AIP-klienten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508370"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatisk klassificering, der ikke fungerer som forventet med AIP-klienten

Automatisk klassificering ikke opfører sig som forventet, skal du bruge følgende anbefalede retningslinjer:

1. Hvis du har problemer med automatisk mærkning, skal du se [Sådan konfigureres betingelserne for automatisk og anbefalet klassificering af Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og [hvad de følsomme oplysningstyper søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Kontrollér, om du bruger scoped-politikker, der ikke er konfigureret korrekt: [Sådan konfigureres politikken for Azure Information Protection for bestemte brugere ved hjælp af politikker for omfang](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Hvis automatisk mærkning ikke fungerer for Outlook, når du vedhæfter et navngivet dokument, skal du kontrollere, at det `DRMEncryptProperty` ikke er defineret som beskrevet her: [IRM-registreringsdatabaseindstillinger for sikkerhed](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Hvis du har brugt de [indbyggede oplysningstyper til](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) din politik til Beskyttelse af Azure Information, skal du kontrollere, at dit indhold svarer til det forventede format.
5. Kontroller, at etiketten er konfigureret korrekt til **Automatisk** eller **Anbefalet**. **(Automatisk** mærkning er tilgængelig for alle Office-apps, mens **Anbefalet** er tilgængelig for alle Office-apps undtagen Outlook).
6. Du kan ikke bruge automatisk klassificering til dokumenter og mails, der tidligere var manuelt mærket eller tidligere automatisk mærket med en højere klassificering.  Du kan finde flere oplysninger under: [Sådan anvendes automatiske eller anbefalede etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Hvis du stadig oplever problemer, skal du indsamle Azure Information Protection-klientlogfiler og vedhæfte de eksporterede logfiler til din supportbillet. Sådan eksporteres Azure Information Protection-logfiler:
    - Åbn et Office-dokument, eller opret en ny mail i Outlook.
    - Klik på **Hjælp til beskyttelse/følsomhed**  >  **og feedback**.
    - Klik på **Eksportér logfiler**.
    - Gem logfilerne til dit valg af placering, og vedhæft dem til din serviceanmodning.

Yderligere oplysninger finder du i:

- [Sådan konfigureres betingelser for automatisk og anbefalet klassificering af Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Vejledninger til almindelige scenarier, der bruger Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Gennemse dokumentationen til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Gennemse Azure Information Protection-abonnementer og -funktioner](https://azure.microsoft.com/pricing/details/information-protection)
- [Krav til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Selvstudium til hurtig start til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Download Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
