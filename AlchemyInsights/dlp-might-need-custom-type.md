---
title: DLP skal muligvis bruge en brugerdefineret type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712178"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="9f0f2-102">DLP skal muligvis bruge en brugerdefineret type</span><span class="sxs-lookup"><span data-stu-id="9f0f2-102">DLP might need a custom type</span></span>

<span data-ttu-id="9f0f2-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="9f0f2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9f0f2-104">**DLP kræver muligvis en brugerdefineret oplysningstype**</span><span class="sxs-lookup"><span data-stu-id="9f0f2-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="9f0f2-105">Med en politik til forebyggelse af datatab (DLP) kan du identificere og beskytte følsomme data i organisationen.</span><span class="sxs-lookup"><span data-stu-id="9f0f2-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="9f0f2-106">I visse scenarier kan det være nødvendigt at oprette din egen **brugerdefinerede** type fortrolige oplysninger for at beskytte din organisationsdata.</span><span class="sxs-lookup"><span data-stu-id="9f0f2-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="9f0f2-107">For eksempel skal din organisation muligvis identificere og beskytte medarbejder-id'er eller andre data i et hvilket som helst format, der er specifikt for din organisation. Hvis det er tilfældet, skal du se følgende artikler for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="9f0f2-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="9f0f2-108">**Tilpasse en indbygget type af følsomme oplysninger**</span><span class="sxs-lookup"><span data-stu-id="9f0f2-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="9f0f2-109">Hvis en indbygget følsom oplysningstype opfylder dine behov med blot nogle få tilpasninger, kan du [tilpasse en indbygget type af følsomme oplysninger](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="9f0f2-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="9f0f2-110">Du kan f. eks. tilføje eller fjerne nøgleord eller tilføje eller fjerne dokumentation, som f. eks en dato eller adresse.</span><span class="sxs-lookup"><span data-stu-id="9f0f2-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="9f0f2-111">**Oprette en brugerdefineret følsom oplysningstype**</span><span class="sxs-lookup"><span data-stu-id="9f0f2-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="9f0f2-112">Men hvis du har brug for at identificere og beskytte en anden type følsomme oplysninger, kan du [oprette en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i brugergrænsefladen for sikkerheds & overholdelses Center.</span><span class="sxs-lookup"><span data-stu-id="9f0f2-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="9f0f2-113">**Oprette en brugerdefineret følsom oplysningstype i sikkerhed & overholdelses Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="9f0f2-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="9f0f2-114">Hvis BRUGERGRÆNSEFLADEN ikke indeholder alle de indstillinger, du har brug for, kan du [oprette en brugerdefineret følsom oplysningstype i sikkerhed & overholdelses Center-PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9f0f2-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="9f0f2-115">Når du starter med en XML-fil, kan du bruge alle tilgængelige indstillinger.</span><span class="sxs-lookup"><span data-stu-id="9f0f2-115">By starting with an XML file, you can use every option available.</span></span>
