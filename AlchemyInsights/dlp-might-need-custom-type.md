---
title: DLP skal muligvis bruge en brugerdefineret type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932652"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="3d196-102">DLP skal muligvis bruge en brugerdefineret type</span><span class="sxs-lookup"><span data-stu-id="3d196-102">DLP might need a custom type</span></span>

<span data-ttu-id="3d196-103">**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden.</span><span class="sxs-lookup"><span data-stu-id="3d196-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3d196-104">Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="3d196-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3d196-105">I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.</span><span class="sxs-lookup"><span data-stu-id="3d196-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3d196-106">Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage.</span><span class="sxs-lookup"><span data-stu-id="3d196-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3d196-107">Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider.</span><span class="sxs-lookup"><span data-stu-id="3d196-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3d196-108">I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.</span><span class="sxs-lookup"><span data-stu-id="3d196-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3d196-109">**DLP kan kræve en brugerdefineret oplysningstype**</span><span class="sxs-lookup"><span data-stu-id="3d196-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="3d196-110">Med en DLP-politik (Data Loss Prevention) kan du identificere og beskytte følsomme data i organisationen.</span><span class="sxs-lookup"><span data-stu-id="3d196-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="3d196-111">I nogle scenarier skal du muligvis oprette din egen **brugerdefinerede** følsomme oplysningstype for at beskytte organisationens data.</span><span class="sxs-lookup"><span data-stu-id="3d196-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="3d196-112">bruge organisationen til at identificere og beskytte medarbejder-id'er eller andre data i et format, der er specifikt for din organisation. Hvis det er tilfældet, kan du finde flere oplysninger i følgende artikler.</span><span class="sxs-lookup"><span data-stu-id="3d196-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="3d196-113">**Tilpasse en indbygget person af følsomme oplysninger**</span><span class="sxs-lookup"><span data-stu-id="3d196-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="3d196-114">Hvis en indbygget type følsomme oplysninger opfylder dine behov med nogle få justeringer, kan du [tilpasse en indbygget type følsomme oplysninger](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="3d196-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="3d196-115">tilføje eller fjerne søgeord eller tilføje eller fjerne dokumentation, f.eks.</span><span class="sxs-lookup"><span data-stu-id="3d196-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="3d196-116">**Oprette en brugerdefineret følsom oplysningstype**</span><span class="sxs-lookup"><span data-stu-id="3d196-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="3d196-117">Men hvis du har brug for helt at identificere og beskytte en anden type følsomme oplysninger, kan du [oprette en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i brugergrænsefladen i Sikkerheds& Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="3d196-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="3d196-118">**Oprette en brugerdefineret følsom oplysningstype i Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="3d196-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="3d196-119">Hvis brugergrænsefladen ikke indeholder alle de indstillinger, du har brug for, kan du [oprette en brugerdefineret følsom oplysningstype i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="3d196-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="3d196-120">Ved at starte med en XML-fil kan du bruge alle tilgængelige indstillinger.</span><span class="sxs-lookup"><span data-stu-id="3d196-120">By starting with an XML file, you can use every option available.</span></span>
