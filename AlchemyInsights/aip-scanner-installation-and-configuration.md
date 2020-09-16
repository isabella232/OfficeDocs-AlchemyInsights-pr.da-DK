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
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="2f50f-102">AIP scanner: installation og konfiguration</span><span class="sxs-lookup"><span data-stu-id="2f50f-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="2f50f-103">**Hvis du vil installere AIP-scanneren, skal du følge de anbefalede retningslinjer**:</span><span class="sxs-lookup"><span data-stu-id="2f50f-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="2f50f-104">Hvis du er ved at opgradere og ikke udfører en ren installation, skal du kontrollere, at du har fulgt retningslinjerne for [opgradering af Azure information Protection-scanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for Unified labels-klienten, under [opgradering af scanneren til Azure-informations beskyttelse](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="2f50f-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="2f50f-105">Kontrollér, at du er i overensstemmelse med alle [firewall-og netværksinfrastruktur krav](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="2f50f-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="2f50f-106">Sørg for, at dine [politikker er angivet](https://docs.microsoft.com/azure/information-protection/configure-policy) til automatisk mærkning eller har en standardetiket i politikken.</span><span class="sxs-lookup"><span data-stu-id="2f50f-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="2f50f-107">Sørg for, at den relevante filtype er konfigureret til etiket/beskyttelse som beskrevet i [de filtyper, der understøttes af Azure information Protection-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="2f50f-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="2f50f-108">Hvis du også vil ændre standardfunktionsmåden, skal du følge disse retningslinjer: [ændring af standardbeskyttelsesniveauet for filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="2f50f-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="2f50f-109">Kontrollér, at den brugerkonto, der er konfigureret til at køre scanner tjenesten, har tilladelse til at få adgang til alle de konfigurerede lagre.</span><span class="sxs-lookup"><span data-stu-id="2f50f-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="2f50f-110">Hvis du stadig oplever problemer, skal du eksportere scanner loggene og føje dem til din support billet.</span><span class="sxs-lookup"><span data-stu-id="2f50f-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="2f50f-111">**Eksportere scannings logfiler for Azure information Protection**</span><span class="sxs-lookup"><span data-stu-id="2f50f-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="2f50f-112">Gå til%localappdata%\Microsoft\MSIP under den brugerkontekst, der kører scanner tjenesten.</span><span class="sxs-lookup"><span data-stu-id="2f50f-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="2f50f-113">Zip alt indhold under mappen MSIP</span><span class="sxs-lookup"><span data-stu-id="2f50f-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="2f50f-114">Gem logfilerne til dit valg af placering, og knyt dem til din serviceanmodning.</span><span class="sxs-lookup"><span data-stu-id="2f50f-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="2f50f-115">Du kan også bruge [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="2f50f-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="2f50f-116">**Du kan finde flere oplysninger i**:</span><span class="sxs-lookup"><span data-stu-id="2f50f-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="2f50f-117">Installation af Azure information Protection scanner til automatisk at klassificere og beskytte filer</span><span class="sxs-lookup"><span data-stu-id="2f50f-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="2f50f-118">Angive og bruge parameteren token til set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="2f50f-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="2f50f-119">Køre en registrerings cyklus og få vist rapporter for scanneren</span><span class="sxs-lookup"><span data-stu-id="2f50f-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="2f50f-120">Gennemgå dokumentationen til Azure information Protection</span><span class="sxs-lookup"><span data-stu-id="2f50f-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="2f50f-121">Krav til Azure information Protection</span><span class="sxs-lookup"><span data-stu-id="2f50f-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="2f50f-122">Hent Azure information Protection-klient</span><span class="sxs-lookup"><span data-stu-id="2f50f-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
