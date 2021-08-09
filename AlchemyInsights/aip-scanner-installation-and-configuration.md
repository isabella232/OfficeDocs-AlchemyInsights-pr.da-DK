---
title: 'AIP-scanner: installation og konfiguration'
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
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934251"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP-scanner: installation og konfiguration

**For at installere AIP-scanneren skal du følge de anbefalede retningslinjer:**

1. Hvis du opgraderer og ikke udfører en ren installation, skal du kontrollere, at du har fulgt retningslinjerne for opgradering af [Azure Information Protection-scanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for samlet etiketklient under Opgradering af [Azure Information Protection-scanneren](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Kontrollér, at du overholder alle [krav til Firewalls og indstillinger for netværksinfrastruktur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Sørg for, [at dine politikker er](https://docs.microsoft.com/azure/information-protection/configure-policy) indstillet til automatisk mærkat eller har et standardnavn i politikken.
4. Sørg for, at den relevante filtype er konfigureret til etiket/beskyttelse som beskrevet i Filtyper, der [understøttes af Azure Information Protection-klienten.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Hvis du vil ændre standardfunktionsmåden, skal du desuden følge disse retningslinjer: [Ændring af standardbeskyttelsesniveauet for filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Kontrollér, at brugerkontoen, der er konfigureret til at køre scannertjenesten, har tilladelser til at få adgang til alle konfigurerede lagre.
6. Hvis du stadig oplever problemer, skal du eksportere scannerlogfilerne og føje dem til din supportanmodning.

**Eksportér Azure Information Protection Scanner-logfiler**

1. Gå til %localappdata%\Microsoft\MSIP under den brugerkontekst, der kører scannertjenesten.
2. Zip alt indholdet under MSIP-mappen.
3. Gem logfilerne til det sted, du vil gemme dem, og vedhæft dem til din serviceanmodning.
4. Du kan også bruge [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Du kan finde flere oplysninger i:**
- [Installation af Azure Information Protection-scanneren til automatisk at klassificere og beskytte filer](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angive og bruge tokenparameteren for Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Kør en registreringscyklus, og få vist rapporter for scanneren](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Gennemse Azure Information Protection-dokumentation](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav til Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Download Azure Information Protection-klienten](https://www.microsoft.com/download/details.aspx?id=53018)
