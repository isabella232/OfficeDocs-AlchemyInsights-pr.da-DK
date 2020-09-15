---
title: DLP-regel for amerikansk bank kontonummer virker ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679290"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="56d80-102">DLP-problemer med US Bank kontonumre</span><span class="sxs-lookup"><span data-stu-id="56d80-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="56d80-103">**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="56d80-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="56d80-104">**DLP-problemer med US Bank kontonumre**</span><span class="sxs-lookup"><span data-stu-id="56d80-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="56d80-105">Har du problemer med forebyggelse af datatab **(DLP)** , fungerer det ikke for indhold, der indeholder et **amerikansk bank kontonummer** , når du bruger en DLP-følsom oplysningstype i O365?</span><span class="sxs-lookup"><span data-stu-id="56d80-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="56d80-106">Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken ser ud, når den evalueres.</span><span class="sxs-lookup"><span data-stu-id="56d80-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="56d80-107">For eksempel på en politik om et **amerikansk bankkontonummer** konfigureret med et tillidsniveau på 85% evalueres følgende, og du skal registrere, at reglen skal udløse:</span><span class="sxs-lookup"><span data-stu-id="56d80-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="56d80-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre</span><span class="sxs-lookup"><span data-stu-id="56d80-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="56d80-109">**[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 fortløbende cifre.</span><span class="sxs-lookup"><span data-stu-id="56d80-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="56d80-110">**[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen kontrolsum</span><span class="sxs-lookup"><span data-stu-id="56d80-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="56d80-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-politik er 75% sikker på, at den har registreret denne type af følsomme oplysninger, hvis det inden for en afstand af 300 tegn:</span><span class="sxs-lookup"><span data-stu-id="56d80-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="56d80-112">Det regulære udtryk Regex_usa_bank_account_number finder indhold, der svarer til mønsteret</span><span class="sxs-lookup"><span data-stu-id="56d80-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="56d80-113">Der er fundet et nøgleord fra Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="56d80-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="56d80-114">Eksempelvis vil den følgende prøve blive udløst for politikken for **US-bankkontonummer** : tjekke konto 78344011</span><span class="sxs-lookup"><span data-stu-id="56d80-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="56d80-115">Hvis du vil have mere at vide om, hvad der kræves for at få et **amerikansk bank kontonummer** til dit indhold, skal du se følgende afsnit i denne artikel: [hvad de følsomme oplysningstyper ser efter US Bank kontonummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="56d80-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="56d80-116">Ved hjælp af en anden indbygget type af følsomme oplysninger, skal du se følgende artikel for oplysninger om, hvad der kræves til andre typer: [hvad de følsomme oplysningstyper ser ud for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="56d80-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  