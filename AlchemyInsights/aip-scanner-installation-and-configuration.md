---
title: 'AIP scanner: installation og konfiguration'
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
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686636"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP scanner: installation og konfiguration

**Hvis du vil installere AIP-scanneren, skal du følge de anbefalede retningslinjer**:

1. Hvis du er ved at opgradere og ikke udfører en ren installation, skal du kontrollere, at du har fulgt retningslinjerne for [opgradering af Azure information Protection-scanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for Unified labels-klienten, under [opgradering af scanneren til Azure-informations beskyttelse](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Kontrollér, at du er i overensstemmelse med alle [firewall-og netværksinfrastruktur krav](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Sørg for, at dine [politikker er angivet](https://docs.microsoft.com/azure/information-protection/configure-policy) til automatisk mærkning eller har en standardetiket i politikken.
4. Sørg for, at den relevante filtype er konfigureret til etiket/beskyttelse som beskrevet i [de filtyper, der understøttes af Azure information Protection-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Hvis du også vil ændre standardfunktionsmåden, skal du følge disse retningslinjer: [ændring af standardbeskyttelsesniveauet for filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Kontrollér, at den brugerkonto, der er konfigureret til at køre scanner tjenesten, har tilladelse til at få adgang til alle de konfigurerede lagre.
6. Hvis du stadig oplever problemer, skal du eksportere scanner loggene og føje dem til din support billet.

**Eksportere scannings logfiler for Azure information Protection**

1. Gå til%localappdata%\Microsoft\MSIP under den brugerkontekst, der kører scanner tjenesten.
2. Zip alt indhold under mappen MSIP
3. Gem logfilerne til dit valg af placering, og knyt dem til din serviceanmodning.
4. Du kan også bruge [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Du kan finde flere oplysninger i**:
- [Installation af Azure information Protection scanner til automatisk at klassificere og beskytte filer](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Angive og bruge parameteren token til set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Køre en registrerings cyklus og få vist rapporter for scanneren](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Gennemgå dokumentationen til Azure information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav til Azure information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hent Azure information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
