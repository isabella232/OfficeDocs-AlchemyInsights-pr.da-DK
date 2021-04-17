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
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821621"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="0c04c-102">AIP: Politikker opfører sig ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="0c04c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="0c04c-103">Azure Information Protection: Politikker opfører sig ikke som forventet, se følgende for anbefalede retningslinjer for forskellige politikproblemer:</span><span class="sxs-lookup"><span data-stu-id="0c04c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="0c04c-104">Hvis du har problemer med visuelle markeringer, skal du gennemse [Når der anvendes visuelle markeringer](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="0c04c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="0c04c-105">Hvis du har problemer med automatisk mærkning, skal du se Sådan konfigurerer du betingelser for automatisk og anbefalet klassificering [af Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og Hvad typerne af følsomme oplysninger søger [efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="0c04c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="0c04c-106">Hvis du har problemer med beskyttelse af native/Pfile, skal du gennemse Konfiguration [af File API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="0c04c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="0c04c-107">Kontrollér, om du bruger omfangsspecifikke politikker, der ikke er konfigureret korrekt: Sådan konfigureres politikken for Azure Information Protection for bestemte brugere ved hjælp af politikker med [omfang.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="0c04c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="0c04c-108">Hvis automatisk mærkning ikke fungerer i Outlook, når du vedhæfter et mærket dokument, skal du kontrollere, at DRMEncryptProperty ikke er defineret som beskrevet her: Indstillinger for [IRM-registreringsdatabasen for](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)sikkerhed .</span><span class="sxs-lookup"><span data-stu-id="0c04c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="0c04c-109">Hvis du stadig oplever problemer, skal du indsamle Azure Information Protection-klientlogfiler og vedhæfte de eksporterede logfiler til denne billet.</span><span class="sxs-lookup"><span data-stu-id="0c04c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="0c04c-110">Åbn et Office-dokument, eller opret en ny mail i Outlook.</span><span class="sxs-lookup"><span data-stu-id="0c04c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="0c04c-111">Klik **på Beskyt/følsomhed**  >  **hjælp og feedback**.</span><span class="sxs-lookup"><span data-stu-id="0c04c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="0c04c-112">Klik **på Eksportér logfiler.**</span><span class="sxs-lookup"><span data-stu-id="0c04c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="0c04c-113">Gem logfilerne til din placering, og vedhæft dem til denne serviceanmodning.</span><span class="sxs-lookup"><span data-stu-id="0c04c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="0c04c-114">Flere ressourcer:</span><span class="sxs-lookup"><span data-stu-id="0c04c-114">Additional resources:</span></span>

- [<span data-ttu-id="0c04c-115">Sådan konfigurerer du en etiket til visuelle markeringer til Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="0c04c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="0c04c-116">Gennemse Azure Information Protection-dokumentation</span><span class="sxs-lookup"><span data-stu-id="0c04c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="0c04c-117">Brug følsomhedsmærkater i Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="0c04c-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

