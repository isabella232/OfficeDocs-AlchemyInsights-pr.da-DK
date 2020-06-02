---
title: DLP skal muligvis bruge en brugerdefineret type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507508"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="3a29d-102">DLP skal muligvis bruge en brugerdefineret type</span><span class="sxs-lookup"><span data-stu-id="3a29d-102">DLP might need a custom type</span></span>

<span data-ttu-id="3a29d-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="3a29d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="3a29d-104">**DLP kan kræve en brugerdefineret informationstype**</span><span class="sxs-lookup"><span data-stu-id="3a29d-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="3a29d-105">Med en DLP-politik (Data Loss Prevention) kan du identificere og beskytte følsomme data i organisationen.</span><span class="sxs-lookup"><span data-stu-id="3a29d-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="3a29d-106">I nogle scenarier skal du muligvis oprette din egen **brugerdefinerede** følsomme oplysningstype for at beskytte organisationens data.</span><span class="sxs-lookup"><span data-stu-id="3a29d-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="3a29d-107">Din organisation kan for eksempel være nødt til at identificere og beskytte medarbejder-id'er eller andre data i et format, der er specifikt for din organisation. Hvis det er tilfældet, kan du finde flere oplysninger i følgende artikler.</span><span class="sxs-lookup"><span data-stu-id="3a29d-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="3a29d-108">**Tilpasse en indbygget følsom oplysningstype**</span><span class="sxs-lookup"><span data-stu-id="3a29d-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="3a29d-109">Hvis en indbygget følsom informationstype opfylder dine behov med blot et par justeringer, kan du [tilpasse en indbygget følsom informationstype](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="3a29d-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="3a29d-110">tilføje eller fjerne nøgleord eller tilføje eller fjerne dokumentation, f.eks.</span><span class="sxs-lookup"><span data-stu-id="3a29d-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="3a29d-111">**Oprette en brugerdefineret følsom oplysningstype**</span><span class="sxs-lookup"><span data-stu-id="3a29d-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="3a29d-112">Men hvis du har brug for at identificere og beskytte en anden type følsomme oplysninger helt, kan du [oprette en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i brugergrænsefladen i Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="3a29d-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="3a29d-113">**Oprette en brugerdefineret følsom oplysningstype i Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="3a29d-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="3a29d-114">Hvis brugergrænsefladen ikke indeholder alle de indstillinger, du har brug for, kan du [oprette en brugerdefineret følsom oplysningstype i Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="3a29d-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="3a29d-115">Ved at starte med en XML-fil kan du bruge alle tilgængelige indstillinger.</span><span class="sxs-lookup"><span data-stu-id="3a29d-115">By starting with an XML file, you can use every option available.</span></span>
