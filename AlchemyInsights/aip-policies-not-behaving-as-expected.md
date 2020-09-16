---
title: 'AIP: politikker opfører sig ikke som forventet'
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
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663183"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politikker opfører sig ikke som forventet

Azure information Protection: politikker, der ikke opfører sig som forventet, kan du se følgende for at få anbefalede retningslinjer for forskellige politik problemer:

1. Hvis du har problemer med visuelle påskrifter, skal du gennemgå, [når der anvendes visuelle påskrifter](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Hvis du har problemer med automatisk mærkning, kan du se [, hvordan du konfigurerer betingelserne for automatisk og anbefalet klassificering til Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) , og [hvad de følsomme oplysningstyper ser ud](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Hvis du har problemer med indbygget/Pfile beskyttelse, skal du gennemgå [konfiguration af fil-API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontrollér, om du brugerområde politikker, der ikke er konfigureret korrekt: [Sådan konfigurerer du politikken for Azure-informations beskyttelse for bestemte brugere ved hjælp af område politikker](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Hvis automatisk mærkning ikke fungerer i Outlook, når du vedhæfter et mærket dokument, skal du kontrollere, at DRMEncryptProperty ikke er defineret som beskrevet her: [IRM-registreringsdatabaseindstillinger for sikkerhed](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Hvis du stadig oplever problemer, skal du indsamle en anmodning om at indsamle en klient til Azure information Protection og vedhæfte de eksporterede logfiler til denne billet.

1. Åbn et Office-dokument, eller Opret en ny mail i Outlook.
2. Klik på **Beskyt/følsomhed**  >  **Hjælp og feedback**.
3. Klik på **Eksportér logfiler**.
4. Gem logfilerne til dit valg af placering, og Vedhæft dem til denne serviceanmodning.

Flere ressourcer:

- [Sådan konfigureres en etiket for visuelle mærker til Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Gennemgå dokumentationen til Azure information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Brug følsomheds etiketter i Microsoft 365-apps](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

