---
title: 'AIP: Politikker, der ikke fungerer som forventet'
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
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/26/2020
ms.locfileid: "44492955"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politikker, der ikke fungerer som forventet

Azure Information Protection: Politikker, der ikke fungerer som forventet, kan se følgende for at få anbefalede retningslinjer for forskellige politikproblemer:

1. Hvis du har problemer med visuelle markeringer, skal du gennemse [Når der anvendes visuelle markeringer](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Hvis du har problemer med automatisk mærkning, skal du se Sådan konfigurerer du [betingelser for automatisk og anbefalet klassificering af Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og hvad de følsomme [oplysningstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
3. Hvis du har problemer med indbygget/p-fil-beskyttelse, skal du gennemse [Fil-API-konfigurationen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Kontrollér, om du bruger scoped-politikker, der ikke er konfigureret korrekt: [Sådan konfigureres politikken for Azure Information Protection for bestemte brugere ved hjælp af politikker for omfang](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Hvis automatisk mærkning ikke fungerer for Outlook, når du vedhæfter et navngivet dokument, skal du kontrollere, at DRMEncryptProperty ikke er defineret som beskrevet her: [IRM-registreringsdatabaseindstillinger for sikkerhed](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Hvis du stadig oplever problemer, skal du indsamle Azure Information Protection-klientlogfiler og vedhæfte de eksporterede logfiler til denne billet.

1. Åbn et Office-dokument, eller opret en ny mail i Outlook.
2. Klik på **Hjælp til beskyttelse/følsomhed**  >  **og feedback**.
3. Klik på **Eksportér logfiler**.
4. Gem logfilerne til dit valg af placering, og vedhæft dem til denne serviceanmodning.

Flere ressourcer:

- [Sådan konfigureres en etiket til visuelle markeringer for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Gennemse dokumentationen til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bruge følsomhedsetiketter i Office-apps](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

