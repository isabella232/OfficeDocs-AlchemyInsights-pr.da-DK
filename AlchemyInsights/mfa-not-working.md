---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755125"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="94b94-102">Problemer med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="94b94-102">Issues with Azure MFA</span></span>
<span data-ttu-id="94b94-103">Der er et par ting, du skal kontrollere, hvis brugerne ikke kan logge på ved hjælp af multifaktorgodkendelse (MFA)</span><span class="sxs-lookup"><span data-stu-id="94b94-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="94b94-104">Den pågældende bruger kan være blokeret i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="94b94-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="94b94-105">Hvis det er tilfældet, bliver godkendelsesforsøg for den pågældende bruger automatisk afvist.</span><span class="sxs-lookup"><span data-stu-id="94b94-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="94b94-106">Følg trinnene i denne artikel for at fjerne blokeringen af dem.</span><span class="sxs-lookup"><span data-stu-id="94b94-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="94b94-107">Hvis det ikke hjælper at fjerne blokeringen af brugeren, eller brugeren ikke er blokeret, kan du prøve at nulstille MFA for brugeren, og den gennemgår processen igen.</span><span class="sxs-lookup"><span data-stu-id="94b94-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="94b94-108">Følg trinnene i denne artikel.</span><span class="sxs-lookup"><span data-stu-id="94b94-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="94b94-109">Hvis dette er første gang, du aktiverer MFA, og dine brugere ikke kan logge på ikke-browser-klienter, såsom Outlook, Skype osv., kan ADAL (Active Directory Authentication Library) ikke være aktiveret på dit O365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="94b94-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="94b94-110">I dette tilfælde skal du oprette forbindelse til Exchange Online PowerShell og køre denne cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="94b94-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>