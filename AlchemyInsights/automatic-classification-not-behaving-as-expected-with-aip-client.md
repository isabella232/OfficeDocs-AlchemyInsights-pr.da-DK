---
title: Automatisk klassificering opfører sig ikke som forventet med AIP-klienten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715195"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatisk klassificering opfører sig ikke som forventet med AIP-klienten

Automatisk klassificering opfører sig ikke som forventet, brug følgende anbefalede retningslinjer:

1. Hvis du har problemer med automatisk mærkning, kan du se, [hvordan du konfigurerer betingelser for automatisk og anbefalet klassificering til Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) , og [hvad de følsomme oplysningstyper ser ud](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Kontrollér, om du brugerområde politikker, der ikke er konfigureret korrekt: [Sådan konfigurerer du politikken for Azure-informations beskyttelse for bestemte brugere ved hjælp af område politikker](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Hvis automatisk mærkning ikke fungerer i Outlook, når du vedhæfter et mærket dokument, skal du bekræfte, at det `DRMEncryptProperty` ikke er defineret som beskrevet her: [IRM-registreringsdatabaseindstillinger for sikkerhed](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Hvis du har brugt de [indbyggede oplysningstyper](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) til din Azure information Protection-politik, skal du bekræfte, at dit indhold passer til det forventede format.
5. Kontrollér, at navnet er korrekt konfigureret til **automatisk** eller **anbefalet**. (**Automatisk** mærkning er tilgængelig for alle Microsoft 365-apps, hvorimod **anbefales** til alle Microsoft 365-apps undtagen til Outlook).
6. Du kan ikke bruge automatisk klassificering for dokumenter og mails, der tidligere blev mærket manuelt, eller som automatisk blev mærket med en højere klassificering.  Du kan finde flere oplysninger i: [Sådan anvendes automatiske eller anbefalede etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Hvis du stadig har problemer, skal du indsamle en anmodning om at indsamle en klient og knytte de eksporterede logfiler til din support billet. Sådan eksporterer du Azure Data Protection-logfiler:
    - Åbn et Office-dokument, eller Opret en ny mail i Outlook.
    - Klik på **Beskyt/følsomhed**  >  **Hjælp og feedback**.
    - Klik på **Eksportér logfiler**.
    - Gem logfilerne til dit valg af placering, og knyt dem til din serviceanmodning.

Du kan finde flere oplysninger i:

- [Sådan konfigureres betingelserne for automatisk og anbefalet klassificering til Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Vejledninger til almindelige scenarier, der bruger Azure information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Gennemgå dokumentationen til Azure information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Gennemgå abonnementer og funktioner til Azure-informations beskyttelse](https://azure.microsoft.com/pricing/details/information-protection)
- [Krav til Azure information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Startvejledning til hurtig start til Azure information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Hent Azure information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
