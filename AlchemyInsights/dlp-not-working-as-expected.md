---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977432"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="d9b4d-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="d9b4d-102">DLP not working as expected</span></span>

<span data-ttu-id="d9b4d-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d9b4d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="d9b4d-104">**Opsætning af DLP**</span><span class="sxs-lookup"><span data-stu-id="d9b4d-104">**Setting up DLP**</span></span>

<span data-ttu-id="d9b4d-105">Har du problemer med **Forebyggelse af datatab (DLP)** i Office 365 fungerer ikke som forventet?</span><span class="sxs-lookup"><span data-stu-id="d9b4d-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="d9b4d-106">Hvis det er tilfældet, skal du sørge for, at **DLP-politikken** er konfigureret korrekt, og at dine data indeholder, hvad **DLP-politikken** søger efter, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="d9b4d-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="d9b4d-107">DLP-politikker giver dig mulighed for at identificere og beskytte følsomme oplysninger i organisationen.</span><span class="sxs-lookup"><span data-stu-id="d9b4d-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="d9b4d-108">Hvis du vil konfigurere DLP-politikker, skal du bruge oplysningerne [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="d9b4d-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="d9b4d-109">**Hvad DLP politikker kigge efter**</span><span class="sxs-lookup"><span data-stu-id="d9b4d-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="d9b4d-110">Når dlp-politikker bruger de **indbyggede følsomme oplysningstyper** i Office 365 Security and Compliance Center, søger de specifikke mønstre og elementer, når du registrerer disse følsomme typer.</span><span class="sxs-lookup"><span data-stu-id="d9b4d-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="d9b4d-111">**Indbyggede følsomme oplysningstyper**</span><span class="sxs-lookup"><span data-stu-id="d9b4d-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="d9b4d-112">Du kan finde oplysninger om de indbyggede følsomme typer, og hvad en DLP-politik søger efter, når du registrerer typen Følsom, under: [Hvad de følsomme oplysningstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="d9b4d-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="d9b4d-113">**Brugerdefinerede følsomme oplysningstyper**</span><span class="sxs-lookup"><span data-stu-id="d9b4d-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="d9b4d-114">Hvis du forsøger at oprette brugerdefinerede følsomme oplysningstyper, kan du bruge følgende artikel til at få oplysninger om, hvordan du opretter en brugerdefineret følsom type: [Opret en brugerdefineret personfølsomme oplysningertype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d9b4d-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="d9b4d-115">**Test en DLP-politik**</span><span class="sxs-lookup"><span data-stu-id="d9b4d-115">**Test a DLP policy**</span></span>

<span data-ttu-id="d9b4d-116">Hvis du vil teste dine data med en indbygget eller brugerdefineret følsom oplysningstype, skal du bruge indstillingen **Testtype** under **Klassifikationer** > **Følsomme oplysningstyper**.</span><span class="sxs-lookup"><span data-stu-id="d9b4d-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="d9b4d-117">Yderligere oplysninger finder du i [Test af brugerdefinerede følsomme oplysningstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="d9b4d-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="d9b4d-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="d9b4d-118">**Reports**</span></span>
  
- <span data-ttu-id="d9b4d-119">Få indsigt i følsomme data med [DLP-rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="d9b4d-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="d9b4d-120">Se specifikke oplysninger om hændelsen med en [hændelsesrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="d9b4d-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
