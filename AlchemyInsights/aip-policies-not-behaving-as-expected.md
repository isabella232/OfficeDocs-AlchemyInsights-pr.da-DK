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
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="4385a-102">AIP: politikker opfører sig ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="4385a-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="4385a-103">Azure information Protection: politikker, der ikke opfører sig som forventet, kan du se følgende for at få anbefalede retningslinjer for forskellige politik problemer:</span><span class="sxs-lookup"><span data-stu-id="4385a-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="4385a-104">Hvis du har problemer med visuelle påskrifter, skal du gennemgå, [når der anvendes visuelle påskrifter](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="4385a-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="4385a-105">Hvis du har problemer med automatisk mærkning, kan du se [, hvordan du konfigurerer betingelserne for automatisk og anbefalet klassificering til Azure information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) , og [hvad de følsomme oplysningstyper ser ud](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="4385a-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="4385a-106">Hvis du har problemer med indbygget/Pfile beskyttelse, skal du gennemgå [konfiguration af fil-API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="4385a-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="4385a-107">Kontrollér, om du brugerområde politikker, der ikke er konfigureret korrekt: [Sådan konfigurerer du politikken for Azure-informations beskyttelse for bestemte brugere ved hjælp af område politikker](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="4385a-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="4385a-108">Hvis automatisk mærkning ikke fungerer i Outlook, når du vedhæfter et mærket dokument, skal du kontrollere, at DRMEncryptProperty ikke er defineret som beskrevet her: [IRM-registreringsdatabaseindstillinger for sikkerhed](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="4385a-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="4385a-109">Hvis du stadig oplever problemer, skal du indsamle en anmodning om at indsamle en klient til Azure information Protection og vedhæfte de eksporterede logfiler til denne billet.</span><span class="sxs-lookup"><span data-stu-id="4385a-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="4385a-110">Åbn et Office-dokument, eller Opret en ny mail i Outlook.</span><span class="sxs-lookup"><span data-stu-id="4385a-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="4385a-111">Klik på **Beskyt/følsomhed**  >  **Hjælp og feedback**.</span><span class="sxs-lookup"><span data-stu-id="4385a-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="4385a-112">Klik på **Eksportér logfiler**.</span><span class="sxs-lookup"><span data-stu-id="4385a-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="4385a-113">Gem logfilerne til dit valg af placering, og Vedhæft dem til denne serviceanmodning.</span><span class="sxs-lookup"><span data-stu-id="4385a-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="4385a-114">Flere ressourcer:</span><span class="sxs-lookup"><span data-stu-id="4385a-114">Additional resources:</span></span>

- [<span data-ttu-id="4385a-115">Sådan konfigureres en etiket for visuelle mærker til Azure information Protection</span><span class="sxs-lookup"><span data-stu-id="4385a-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="4385a-116">Gennemgå dokumentationen til Azure information Protection</span><span class="sxs-lookup"><span data-stu-id="4385a-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="4385a-117">Brug følsomheds etiketter i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="4385a-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

