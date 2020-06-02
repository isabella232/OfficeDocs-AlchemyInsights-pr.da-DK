---
title: DLP-regel for pasnummer i USA/Storbritannien fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507292"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="6aa44-102">Problemer med DLP - USA/Storbritannien pasnumre</span><span class="sxs-lookup"><span data-stu-id="6aa44-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="6aa44-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="6aa44-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6aa44-104">**DLP problemer med USA / UK pasnumre**</span><span class="sxs-lookup"><span data-stu-id="6aa44-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="6aa44-105">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke arbejder for indhold, der indeholder et **amerikansk/britisk pasnummer,** når du bruger en DLP-følsom informationstype i O365?</span><span class="sxs-lookup"><span data-stu-id="6aa44-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="6aa44-106">Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken søger efter, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="6aa44-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="6aa44-107">For en politik for pasnummer i **USA/Storbritannien,** der er konfigureret med et konfidensniveau på 75 %, evalueres følgende og skal registreres, for at reglen kan udløses</span><span class="sxs-lookup"><span data-stu-id="6aa44-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="6aa44-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni cifre</span><span class="sxs-lookup"><span data-stu-id="6aa44-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="6aa44-109">**[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni cifre i træk</span><span class="sxs-lookup"><span data-stu-id="6aa44-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="6aa44-110">**[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen Checksum</span><span class="sxs-lookup"><span data-stu-id="6aa44-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="6aa44-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-politik er 75 % sikker på, at den registreres denne type følsomme oplysninger, hvis den er i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="6aa44-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6aa44-112">Funktionen Func_usa_uk_passport finder indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="6aa44-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="6aa44-113">Der blev fundet et nøgleord fra Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="6aa44-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="6aa44-114">For eksempel vil følgende prøve udløse for **den amerikanske / britiske pas nummer** politik: US Passport nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="6aa44-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="6aa44-115">Du kan finde flere oplysninger om, hvad der kræves for at få registreret et amerikansk/britisk passport-nummer for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme informationstyper søger efter amerikansk/britisk passport-nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="6aa44-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="6aa44-116">Brug af en anden indbygget følsom oplysningstype i følgende artikel for at få oplysninger om, hvad der kræves til andre typer: [Hvad de følsomme oplysninger søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="6aa44-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  