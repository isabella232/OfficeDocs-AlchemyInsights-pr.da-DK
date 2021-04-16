---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810478"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="2020a-102">Problemer med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="2020a-102">Issues with Azure MFA</span></span>
<span data-ttu-id="2020a-103">Der er et par ting, der skal kontrolleres, hvis brugerne ikke kan logge på med multifaktorgodkendelse (MFA)</span><span class="sxs-lookup"><span data-stu-id="2020a-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="2020a-104">Den pågældende bruger kan blive blokeret i Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="2020a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="2020a-105">Hvis det er tilfældet, nægtes godkendelsesforsøg for den pågældende bruger automatisk.</span><span class="sxs-lookup"><span data-stu-id="2020a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="2020a-106">Følg trinnene i denne artikel for at fjerne blokeringen af dem.</span><span class="sxs-lookup"><span data-stu-id="2020a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="2020a-107">Hvis det ikke virkede at fjerne blokeringen af brugeren, eller brugeren ikke er blokeret, kan du prøve at nulstille MFA for brugeren, så vil brugeren gå gennem tilmeldingsprocessen igen.</span><span class="sxs-lookup"><span data-stu-id="2020a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="2020a-108">Følg trinnene i denne artikel.</span><span class="sxs-lookup"><span data-stu-id="2020a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="2020a-109">Hvis det er første gang, du har aktiveret MFA, og dine brugere ikke kan logge på klienter, der ikke er i en browser, f.eks. Outlook, Skype osv., er ADAL (Active Directory Authentication Library) ikke aktiveret på dit O365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="2020a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="2020a-110">I dette tilfælde skal du oprette forbindelse til Exchange Online Powershell og køre denne cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="2020a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>