---
title: DLP-regel for kreditkortnummer virker ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404479"
---
<span data-ttu-id="a18f8-102">Har du problemer med **Data tab forebyggelse (DLP)** ikke arbejder for indhold, der indeholder et **Kreditkortnummer** , når du bruger typen DLP følsomme oplysninger i O365?</span><span class="sxs-lookup"><span data-stu-id="a18f8-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a18f8-103">I så fald sikre, at indholdet indeholder de nødvendige oplysninger til at udløse den DLP-politik, når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="a18f8-103">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="a18f8-104">For eksempel for en **politik for kreditkort** , der er konfigureret med et konfidensniveau på 85%, følgende evalueres, og skal registreres for reglen, der udløser:</span><span class="sxs-lookup"><span data-stu-id="a18f8-104">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="a18f8-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre, hvilket kan være formateret eller uformateret (dddddddddddddddd) og skal bestå testen Luhn.</span><span class="sxs-lookup"><span data-stu-id="a18f8-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="a18f8-106">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Meget komplekse og robust mønster, som registrerer kort fra alle større mærker i hele verden, herunder Visa, Mastercard, opdage kort, JCB, American Express, gavekort og diner kort.</span><span class="sxs-lookup"><span data-stu-id="a18f8-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="a18f8-107">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-kontrolsum</span><span class="sxs-lookup"><span data-stu-id="a18f8-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="a18f8-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-politik er 85% sikker på, at det har fundet denne type af følsomme oplysninger, hvis, inden for en afstand af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="a18f8-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="a18f8-109">Funktionen Func_credit_card søger efter indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="a18f8-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="a18f8-110">En af følgende er sandt:</span><span class="sxs-lookup"><span data-stu-id="a18f8-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="a18f8-111">Der findes et nøgleord fra Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="a18f8-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="a18f8-112">Der findes et nøgleord fra Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="a18f8-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="a18f8-113">Funktionen Func_expiration_date findes en dato i det rigtige format.</span><span class="sxs-lookup"><span data-stu-id="a18f8-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="a18f8-114">Kontrolsummen overføres</span><span class="sxs-lookup"><span data-stu-id="a18f8-114">The checksum passes</span></span>
    
    <span data-ttu-id="a18f8-115">For eksempel vil følgende eksempel udløse en DLP kreditkort nummer politik:</span><span class="sxs-lookup"><span data-stu-id="a18f8-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="a18f8-116">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="a18f8-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="a18f8-117">Udløber: 2-2009</span><span class="sxs-lookup"><span data-stu-id="a18f8-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="a18f8-118">Yderligere oplysninger om, hvad der kræves for et **Kreditkortnummer** og registreres af dit indhold, kan du se følgende afsnit i denne artikel: [Hvad den følsomme oplysningstyper søge efter kreditkort #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="a18f8-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="a18f8-119">Bruge en anden indbygget følsomme oplysninger, se følgende artikel for at få oplysninger om hvad der kræves for andre typer: [Hvad den følsomme oplysningstyper søge efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a18f8-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

