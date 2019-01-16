---
title: DLP-regel for os bankkontonummer virker ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283516"
---
<span data-ttu-id="dd437-p101">Har du problemer med **Data tab forebyggelse (DLP)** ikke arbejder for indhold, der indeholder et **Amerikansk bankkontonummer** , når du bruger typen DLP følsomme oplysninger i O365? Hvis det er tilfældet, skal du sørge for dit indhold indeholder de nødvendige oplysninger for det DLP-Gruppepolitik er søger efter, når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="dd437-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="dd437-104">For eksempel for en **Amerikansk bankkontonummer** politik, der er konfigureret med et konfidensniveau på 85%, følgende evalueres, og skal registreres for reglen, der udløser:</span><span class="sxs-lookup"><span data-stu-id="dd437-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="dd437-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="dd437-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="dd437-106">**[Mønster:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 på hinanden følgende cifre.</span><span class="sxs-lookup"><span data-stu-id="dd437-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="dd437-107">**[Kontrolsum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, der er ingen kontrolsum</span><span class="sxs-lookup"><span data-stu-id="dd437-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="dd437-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** En DLP-politik er 75% sikker på, at det har fundet denne type af følsomme oplysninger, hvis, inden for en afstand af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="dd437-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="dd437-109">Det regulære udtryk Regex_usa_bank_account_number søger efter indhold, der svarer til mønsteret</span><span class="sxs-lookup"><span data-stu-id="dd437-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="dd437-110">Der findes et nøgleord fra Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="dd437-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="dd437-111">For eksempel vil udløse følgende eksempel for den **Amerikanske bankkontonummer** politik: checkkonto 78344011</span><span class="sxs-lookup"><span data-stu-id="dd437-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="dd437-112">Yderligere oplysninger om, hvad der kræves for et **Amerikansk bankkontonummeret** skal registreres for dit indhold, kan du se følgende afsnit i denne artikel: [Hvad den følsomme oplysningstyper søge efter Amerikansk bankkonto tal](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="dd437-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="dd437-113">Bruge en anden indbygget følsomme oplysninger, se følgende artikel for at få oplysninger om hvad der kræves for andre typer: [Hvad den følsomme oplysningstyper søge efter](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dd437-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

