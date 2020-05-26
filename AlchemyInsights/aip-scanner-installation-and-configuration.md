---
title: 'AIP-scanner: installation og konfiguration'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357665"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-scanner: installation og konfiguration

**Hvis du vil installere AIP-scanneren, skal du følge de anbefalede retningslinjer:**

1. Hvis du opgraderer og ikke udfører en ren installation, skal du kontrollere, at du har fulgt retningslinjerne for [opgradering af Azure Information Protection-scanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for unified labeling-klienten, se opgradering af Azure Information [Protection-scanneren](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Kontroller, at du overholder alle [krav til firewalls og netværksinfrastruktur](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Sørg for, at dine [politikker er indstillet](https://docs.microsoft.com/azure/information-protection/configure-policy) til automatisk mærkning eller har en standardetiket i politikken.
4. Kontroller, at den relevante filtype er konfigureret til etiket/beskyttelse som beskrevet i [Filtyper, der understøttes af Azure Information Protection-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Hvis du vil ændre standardfunktionsmåden, skal du desuden følge disse retningslinjer: [Ændre standardniveauet for beskyttelse af filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Kontroller, at den brugerkonto, der er konfigureret til at køre scannertjenesten, har tilladelse til at få adgang til alle de konfigurerede lagre.
6. Hvis du stadig oplever problemer, skal du eksportere scannerloggene og føje dem til din supportbillet.

**Eksportere Azure Information Protection Scanner-logfiler**

1. Gå til %localappdata%\Microsoft\MSIP under den brugerkontekst, der kører scannertjenesten.
2. Zip alt indhold under MSIP mappe.
3. Gem logfilerne på dit valg af placering, og vedhæft dem til din serviceanmodning.
4. Du kan også bruge [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Yderligere oplysninger finder du i**:
- [Installation af Azure Information Protection-scanneren til automatisk klassificering og beskyttelse af filer](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angive og bruge tokenparameteren til Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Køre en registreringscyklus, og få vist rapporter for scanneren](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Gennemse dokumentationen til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hent Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
