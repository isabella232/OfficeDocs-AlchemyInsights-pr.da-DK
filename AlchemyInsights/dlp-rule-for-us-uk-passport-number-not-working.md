---
title: DLP-regel for US / UK pasnummer virker ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404375"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c06cb-102">Problemer med DLP - US / UK Passport tal</span><span class="sxs-lookup"><span data-stu-id="c06cb-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="c06cb-103">Du har problemer med **Data tab forebyggelse (DLP)** ikke arbejder for indhold, der indeholder en **US / UK pasnummer** ved brug af typen DLP følsomme oplysninger i O365?</span><span class="sxs-lookup"><span data-stu-id="c06cb-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c06cb-104">Hvis det er tilfældet, skal du sørge for dit indhold indeholder de nødvendige oplysninger for det DLP-Gruppepolitik er søger efter, når det evalueres.</span><span class="sxs-lookup"><span data-stu-id="c06cb-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="c06cb-105">Eksempelvis en **US / UK pasnummer** politik, der er konfigureret med et konfidensniveau på 75%, følgende evalueres og skal registreres for reglen, der udløser</span><span class="sxs-lookup"><span data-stu-id="c06cb-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="c06cb-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Ni cifre</span><span class="sxs-lookup"><span data-stu-id="c06cb-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="c06cb-107">**[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Ni på hinanden følgende cifre</span><span class="sxs-lookup"><span data-stu-id="c06cb-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="c06cb-108">**[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, der er ingen kontrolsum</span><span class="sxs-lookup"><span data-stu-id="c06cb-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="c06cb-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-politik er 75% sikker på, at det har fundet denne type af følsomme oplysninger, hvis, inden for en afstand af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="c06cb-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="c06cb-110">Funktionen Func_usa_uk_passport søger efter indhold, der svarer til mønsteret.</span><span class="sxs-lookup"><span data-stu-id="c06cb-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="c06cb-111">Der findes et nøgleord fra Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="c06cb-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="c06cb-112">For eksempel vil udløse følgende eksempel den **US / UK pasnummer** politik: amerikansk pas tallet 123456789</span><span class="sxs-lookup"><span data-stu-id="c06cb-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="c06cb-113">Yderligere oplysninger om, hvad der kræves for en Amerikansk / UK pasnummer skal registreres for dit indhold, se følgende afsnit i denne artikel: [hvad de følsomme oplysningstyper udseende til USA / UK pasnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="c06cb-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c06cb-114">Bruge en anden indbygget følsomme oplysninger, se følgende artikel for at få oplysninger om hvad der kræves for andre typer: [Hvad den følsomme oplysningstyper søge efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c06cb-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

