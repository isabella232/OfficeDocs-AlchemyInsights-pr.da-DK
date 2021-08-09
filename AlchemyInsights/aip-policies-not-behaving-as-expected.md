---
title: 'AIP: Politikker opfører sig ikke som forventet'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934287"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politikker opfører sig ikke som forventet

Azure Information Protection: Politikker opfører sig ikke som forventet, se følgende for anbefalede retningslinjer for forskellige politikproblemer:

1. Hvis du har problemer med visuelle markeringer, skal du gennemse [Når der anvendes visuelle markeringer](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Hvis du har problemer med automatisk mærkning, skal du se Sådan konfigurerer du betingelser for automatisk og anbefalet klassificering [af Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og Hvad typerne af følsomme oplysninger søger [efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Hvis du har problemer med beskyttelse af native/Pfile, skal du gennemse Konfiguration [af File API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Kontrollér, om du bruger omfangsspecifikke politikker, der ikke er konfigureret korrekt: Sådan konfigureres politikken for Azure Information Protection for bestemte brugere ved hjælp af politikker med [omfang.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Hvis automatisk mærkning ikke fungerer for Outlook når du vedhæfter et mærket dokument, skal du kontrollere, at DRMEncryptProperty ikke er defineret som beskrevet her: Indstillinger for [IRM-registreringsdatabasen for](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)sikkerhed .

Hvis du stadig oplever problemer, skal du indsamle Azure Information Protection-klientlogfiler og vedhæfte de eksporterede logfiler til denne billet.

1. Åbn et Office dokument, eller opret en ny mail i Outlook.
2. Klik **på Beskyt/følsomhed**  >  **hjælp og feedback**.
3. Klik **på Eksportér logfiler.**
4. Gem logfilerne til din placering, og vedhæft dem til denne serviceanmodning.

Flere ressourcer:

- [Sådan konfigurerer du en etiket til visuelle markeringer til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Gennemse Azure Information Protection-dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Brug følsomhedsmærkater i Microsoft 365 apps](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

