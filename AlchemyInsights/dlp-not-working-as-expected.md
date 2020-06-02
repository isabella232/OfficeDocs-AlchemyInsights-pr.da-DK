---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507472"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="ba64c-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="ba64c-102">DLP not working as expected</span></span>

<span data-ttu-id="ba64c-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ba64c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="ba64c-104">**Opsætning af DLP**</span><span class="sxs-lookup"><span data-stu-id="ba64c-104">**Setting up DLP**</span></span>

<span data-ttu-id="ba64c-105">Har du problemer med **forebyggelse af datatab (DLP)** i Office 365 fungerer ikke som forventet?</span><span class="sxs-lookup"><span data-stu-id="ba64c-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="ba64c-106">Hvis det er tilfældet, skal du sørge for, at **DLP-politikken** er konfigureret korrekt, og at dine data indeholder det, **som DLP-politikken** søger efter, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="ba64c-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="ba64c-107">DLP-politikker giver dig mulighed for at identificere og beskytte følsomme oplysninger i organisationen.</span><span class="sxs-lookup"><span data-stu-id="ba64c-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="ba64c-108">Hvis du vil konfigurere DLP-politikker, skal du bruge oplysningerne [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="ba64c-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="ba64c-109">**Hvad DLP-politikker søger efter**</span><span class="sxs-lookup"><span data-stu-id="ba64c-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="ba64c-110">Når du bruger de **indbyggede følsomme oplysningstyper** i sikkerhedscentrene, søger DLP-politikkerne efter specifikke mønstre og elementer, når disse følsomme typer registreres.</span><span class="sxs-lookup"><span data-stu-id="ba64c-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="ba64c-111">**Indbyggede følsomme informationstyper**</span><span class="sxs-lookup"><span data-stu-id="ba64c-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="ba64c-112">Du kan finde oplysninger om de indbyggede følsomme typer, og hvad en DLP-politik søger efter, når du registrerer typen Følsom, under: [Hvad de følsomme oplysningstyper søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="ba64c-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="ba64c-113">**Brugerdefinerede følsomme oplysningstyper**</span><span class="sxs-lookup"><span data-stu-id="ba64c-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="ba64c-114">Hvis du forsøger at oprette brugerdefinerede følsomme oplysningstyper, skal du bruge følgende artikel til at få oplysninger om, hvordan du opretter en brugerdefineret følsom type: [Opret en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="ba64c-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="ba64c-115">**Test en DLP-politik**</span><span class="sxs-lookup"><span data-stu-id="ba64c-115">**Test a DLP policy**</span></span>

<span data-ttu-id="ba64c-116">Hvis du vil teste dine data med en indbygget eller brugerdefineret følsom oplysningstype, skal du bruge indstillingen **Testtype** under **Klassifikationsfølsomme**  >  **oplysningstyper**.</span><span class="sxs-lookup"><span data-stu-id="ba64c-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="ba64c-117">Yderligere oplysninger finder du i [Test af brugerdefinerede følsomme oplysningstyper](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="ba64c-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="ba64c-118">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="ba64c-118">**Reports**</span></span>
  
- <span data-ttu-id="ba64c-119">Få følsom dataindsigt med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="ba64c-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="ba64c-120">Se specifikke oplysninger om hændelsen med en [hændelsesrapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="ba64c-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
