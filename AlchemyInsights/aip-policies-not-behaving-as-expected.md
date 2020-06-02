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
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="6d0f2-102">AIP: Politikker, der ikke fungerer som forventet</span><span class="sxs-lookup"><span data-stu-id="6d0f2-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="6d0f2-103">Azure Information Protection: Politikker, der ikke fungerer som forventet, kan se følgende for at få anbefalede retningslinjer for forskellige politikproblemer:</span><span class="sxs-lookup"><span data-stu-id="6d0f2-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="6d0f2-104">Hvis du har problemer med visuelle markeringer, skal du gennemse [Når der anvendes visuelle markeringer](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="6d0f2-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="6d0f2-105">Hvis du har problemer med automatisk mærkning, skal du se Sådan konfigurerer du [betingelser for automatisk og anbefalet klassificering af Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og hvad de følsomme [oplysningstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="6d0f2-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="6d0f2-106">Hvis du har problemer med indbygget/p-fil-beskyttelse, skal du gennemse [Fil-API-konfigurationen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="6d0f2-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="6d0f2-107">Kontrollér, om du bruger scoped-politikker, der ikke er konfigureret korrekt: [Sådan konfigureres politikken for Azure Information Protection for bestemte brugere ved hjælp af politikker for omfang](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="6d0f2-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="6d0f2-108">Hvis automatisk mærkning ikke fungerer for Outlook, når du vedhæfter et navngivet dokument, skal du kontrollere, at DRMEncryptProperty ikke er defineret som beskrevet her: [IRM-registreringsdatabaseindstillinger for sikkerhed](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="6d0f2-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="6d0f2-109">Hvis du stadig oplever problemer, skal du indsamle Azure Information Protection-klientlogfiler og vedhæfte de eksporterede logfiler til denne billet.</span><span class="sxs-lookup"><span data-stu-id="6d0f2-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="6d0f2-110">Åbn et Office-dokument, eller opret en ny mail i Outlook.</span><span class="sxs-lookup"><span data-stu-id="6d0f2-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="6d0f2-111">Klik på **Hjælp til beskyttelse/følsomhed**  >  **og feedback**.</span><span class="sxs-lookup"><span data-stu-id="6d0f2-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="6d0f2-112">Klik på **Eksportér logfiler**.</span><span class="sxs-lookup"><span data-stu-id="6d0f2-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="6d0f2-113">Gem logfilerne til dit valg af placering, og vedhæft dem til denne serviceanmodning.</span><span class="sxs-lookup"><span data-stu-id="6d0f2-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="6d0f2-114">Flere ressourcer:</span><span class="sxs-lookup"><span data-stu-id="6d0f2-114">Additional resources:</span></span>

- [<span data-ttu-id="6d0f2-115">Sådan konfigureres en etiket til visuelle markeringer for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6d0f2-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="6d0f2-116">Gennemse dokumentationen til Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="6d0f2-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="6d0f2-117">Bruge følsomhedsetiketter i Office-apps</span><span class="sxs-lookup"><span data-stu-id="6d0f2-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

