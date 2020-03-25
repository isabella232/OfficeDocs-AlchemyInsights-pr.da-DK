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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932616"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="1dea8-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="1dea8-102">DLP not working as expected</span></span>

<span data-ttu-id="1dea8-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="1dea8-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1dea8-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="1dea8-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1dea8-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="1dea8-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1dea8-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="1dea8-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1dea8-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="1dea8-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1dea8-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="1dea8-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="1dea8-109">**Opsætning af DLP**</span><span class="sxs-lookup"><span data-stu-id="1dea8-109">**Setting up DLP**</span></span>

<span data-ttu-id="1dea8-110">Har du problemer med **Forebyggelse af datatab (DLP)** i Office 365 fungerer ikke som forventet?</span><span class="sxs-lookup"><span data-stu-id="1dea8-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="1dea8-111">Hvis det er tilfældet, skal du sørge for, at **DLP-politikken** er konfigureret korrekt, og at dine data indeholder, hvad **DLP-politikken** søger efter, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="1dea8-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="1dea8-112">DLP-politikker giver dig mulighed for at identificere og beskytte følsomme oplysninger i organisationen.</span><span class="sxs-lookup"><span data-stu-id="1dea8-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="1dea8-113">Hvis du vil konfigurere DLP-politikker, skal du bruge oplysningerne [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="1dea8-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="1dea8-114">**Hvad DLP politikker kigge efter**</span><span class="sxs-lookup"><span data-stu-id="1dea8-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="1dea8-115">Når dlp-politikker bruger de **indbyggede følsomme oplysningstyper** i Office 365 Security and Compliance Center, søger de specifikke mønstre og elementer, når du registrerer disse følsomme typer.</span><span class="sxs-lookup"><span data-stu-id="1dea8-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="1dea8-116">**Indbyggede følsomme oplysningstyper**</span><span class="sxs-lookup"><span data-stu-id="1dea8-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="1dea8-117">Du kan finde oplysninger om de indbyggede følsomme typer, og hvad en DLP-politik søger efter, når du registrerer typen Følsom, under: [Hvad de følsomme oplysningstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="1dea8-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="1dea8-118">**Brugerdefinerede følsomme oplysningstyper**</span><span class="sxs-lookup"><span data-stu-id="1dea8-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="1dea8-119">Hvis du forsøger at oprette brugerdefinerede følsomme oplysningstyper, kan du bruge følgende artikel til at få oplysninger om, hvordan du opretter en brugerdefineret følsom type: [Opret en brugerdefineret personfølsomme oplysningertype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1dea8-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="1dea8-120">**Test en DLP-politik**</span><span class="sxs-lookup"><span data-stu-id="1dea8-120">**Test a DLP policy**</span></span>

<span data-ttu-id="1dea8-121">Hvis du vil teste dine data med en indbygget eller brugerdefineret følsom oplysningstype, skal du bruge indstillingen **Testtype** under **Klassifikationer** > **Følsomme oplysningstyper**.</span><span class="sxs-lookup"><span data-stu-id="1dea8-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="1dea8-122">Yderligere oplysninger finder du i [Test af brugerdefinerede følsomme oplysningstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="1dea8-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="1dea8-123">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="1dea8-123">**Reports**</span></span>
  
- <span data-ttu-id="1dea8-124">Få indsigt i følsomme data med [DLP-rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="1dea8-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="1dea8-125">Se specifikke oplysninger om hændelsen med en [hændelsesrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="1dea8-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
