---
title: DLP-regel for kreditkortnummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507400"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="b137e-102">DLP-problemer med kreditkortnumre</span><span class="sxs-lookup"><span data-stu-id="b137e-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="b137e-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="b137e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b137e-104">**DLP-problemer med kreditkortnumre**</span><span class="sxs-lookup"><span data-stu-id="b137e-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="b137e-105">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke arbejder for indhold, der indeholder et **kreditkortnummer,** når du bruger en DLP-følsom oplysningstype i O365?</span><span class="sxs-lookup"><span data-stu-id="b137e-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b137e-106">Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger for at udløse DLP-politikken, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="b137e-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="b137e-107">For en **kreditkortpolitik,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks.</span><span class="sxs-lookup"><span data-stu-id="b137e-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b137e-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre, der kan formateres eller ikke er formateret (dddddddddddddddddd) og skal bestå Luhn-testen.</span><span class="sxs-lookup"><span data-stu-id="b137e-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="b137e-109">**[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Meget komplekst og robust mønster, der registrerer kort fra alle større mærker verden over, herunder Visa, MasterCard, Discover Card, JCB, American Express, gavekort og dinerkort.</span><span class="sxs-lookup"><span data-stu-id="b137e-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="b137e-110">**[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn-kontrolsummen</span><span class="sxs-lookup"><span data-stu-id="b137e-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="b137e-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-politik er 85 % sikker på, at den registreres denne type følsomme oplysninger, hvis den er i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="b137e-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b137e-112">Funktionen finder Func_credit_card indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="b137e-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b137e-113">Et af følgende er sandt:</span><span class="sxs-lookup"><span data-stu-id="b137e-113">One of the following is true:</span></span>

  - <span data-ttu-id="b137e-114">Der blev fundet et nøgleord fra Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="b137e-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="b137e-115">Der blev fundet et nøgleord fra Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="b137e-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="b137e-116">Funktionen Func_expiration_date finder en dato i det rigtige datoformat.</span><span class="sxs-lookup"><span data-stu-id="b137e-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="b137e-117">Kontrolsummet passerer</span><span class="sxs-lookup"><span data-stu-id="b137e-117">The checksum passes</span></span>

    <span data-ttu-id="b137e-118">Følgende eksempel udløser f.eks.</span><span class="sxs-lookup"><span data-stu-id="b137e-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="b137e-119">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="b137e-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="b137e-120">Udløber: 2/2009</span><span class="sxs-lookup"><span data-stu-id="b137e-120">Expires: 2/2009</span></span>

<span data-ttu-id="b137e-121">Du kan finde flere oplysninger om, hvad der kræves for at få registreret et **kreditkortnummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme informationstyper søger efter kreditkort#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="b137e-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="b137e-122">Brug af en anden indbygget følsom oplysningstype i følgende artikel for at få oplysninger om, hvad der kræves til andre typer: [Hvad de følsomme oplysninger søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="b137e-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  