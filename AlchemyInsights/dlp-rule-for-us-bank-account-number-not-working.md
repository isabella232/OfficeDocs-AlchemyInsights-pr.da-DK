---
title: DLP-reglen for det amerikanske bankkontonummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507328"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="f2b36-102">DLP-problemer med amerikanske bankkontonumre</span><span class="sxs-lookup"><span data-stu-id="f2b36-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="f2b36-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="f2b36-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f2b36-104">**DLP-problemer med amerikanske bankkontonumre**</span><span class="sxs-lookup"><span data-stu-id="f2b36-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="f2b36-105">Har du problemer med **Forebyggelse af datatab (DLP),** der ikke arbejder for indhold, der indeholder et **amerikansk bankkontonummer,** når du bruger en DLP-følsom oplysningstype i O365?</span><span class="sxs-lookup"><span data-stu-id="f2b36-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="f2b36-106">Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken søger efter, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="f2b36-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="f2b36-107">For en politik for **et amerikansk bankkontonummer,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende og registreres, for at reglen kan udløses:</span><span class="sxs-lookup"><span data-stu-id="f2b36-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f2b36-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="f2b36-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="f2b36-109">**[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 på hinanden følgende cifre.</span><span class="sxs-lookup"><span data-stu-id="f2b36-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="f2b36-110">**[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen Checksum</span><span class="sxs-lookup"><span data-stu-id="f2b36-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="f2b36-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-politik er 75 % sikker på, at den registreres denne type følsomme oplysninger, hvis den er i nærheden af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="f2b36-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f2b36-112">Det regulære udtryk Regex_usa_bank_account_number finder indhold, der svarer til mønsteret</span><span class="sxs-lookup"><span data-stu-id="f2b36-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="f2b36-113">Der blev fundet et nøgleord fra Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="f2b36-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="f2b36-114">Følgende eksempel udløser f.eks. **US Bank Account Number**</span><span class="sxs-lookup"><span data-stu-id="f2b36-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="f2b36-115">Du kan finde flere oplysninger om, hvad der kræves for at finde et **amerikansk bankkontonummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme oplysninger søger efter amerikanske bankkontonummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="f2b36-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="f2b36-116">Brug af en anden indbygget følsom oplysningstype i følgende artikel for at få oplysninger om, hvad der kræves til andre typer: [Hvad de følsomme oplysninger søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="f2b36-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  