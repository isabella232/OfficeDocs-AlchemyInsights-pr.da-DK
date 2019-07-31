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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941062"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="835cd-102">DLP fungerer ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="835cd-102">DLP not working as expected</span></span>

<span data-ttu-id="835cd-103">Du har problemer med **Data tab forebyggelse (DLP)** i Office 365, fungerer ikke som forventet?</span><span class="sxs-lookup"><span data-stu-id="835cd-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="835cd-104">I så fald sikre, at din **DLP-Gruppepolitik** er konfigureret korrekt, og, at dine data indeholder hvilke **DLP-Gruppepolitik** søger efter, når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="835cd-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="835cd-105">**Opsætning af DLP**</span><span class="sxs-lookup"><span data-stu-id="835cd-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="835cd-106">DLP-politikker gør det muligt at identificere og beskytte følsomme oplysninger i din organisation.</span><span class="sxs-lookup"><span data-stu-id="835cd-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="835cd-107">DLP rapportopsætning, skal du bruge oplysningerne [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="835cd-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="835cd-108">**Se hvilke DLP politikker**</span><span class="sxs-lookup"><span data-stu-id="835cd-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="835cd-109">Når du bruger de **indbyggede følsomme oplysningstyper** i Office 365 sikkerhed og kompatibilitet center, se DLP politikker for bestemte mønstre og elementer, når registrering af disse følsomme typer.</span><span class="sxs-lookup"><span data-stu-id="835cd-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="835cd-110">**Typer af indbyggede følsomme oplysninger**</span><span class="sxs-lookup"><span data-stu-id="835cd-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="835cd-111">Finde oplysninger på de følsomme indbyggede typer og en politik for DLP ser når registrering af typen følsomme: [de følsomme oplysninger hvilke ser ud](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="835cd-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="835cd-112">**Typer brugerdefinerede følsomme oplysninger**</span><span class="sxs-lookup"><span data-stu-id="835cd-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="835cd-113">Hvis du forsøger at oprette brugerdefinerede følsomme oplysninger, kan du bruge følgende artikel oplysninger om, hvordan du opretter en brugerdefineret følsomme type: [Opret en brugerdefineret følsomme oplysninger-typen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="835cd-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="835cd-114">**Teste en DLP-politik**</span><span class="sxs-lookup"><span data-stu-id="835cd-114">**Test a DLP policy**</span></span>

<span data-ttu-id="835cd-115">For at teste dine data med en indbygget eller brugerdefineret følsomme oplysninger, skal du bruge indstillingen **Test type** under **klassifikationer** > **typer af følsomme oplysninger**.</span><span class="sxs-lookup"><span data-stu-id="835cd-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="835cd-116">Yderligere oplysninger finder du under [testtyper brugerdefinerede følsomme oplysninger](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="835cd-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="835cd-117">**Rapporter**</span><span class="sxs-lookup"><span data-stu-id="835cd-117">**Reports**</span></span>
  
- <span data-ttu-id="835cd-118">Få indblik i følsomme data med [rapporter DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="835cd-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="835cd-119">Se bestemte oplysninger om hændelsen med en [Hændelse rapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="835cd-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
