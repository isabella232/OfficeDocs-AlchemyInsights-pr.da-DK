---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768831"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="cd435-102">Problemer med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="cd435-102">Issues with Azure MFA</span></span>
<span data-ttu-id="cd435-103">Der er et par ting, du skal kontrollere, hvis brugerne ikke kan logge på ved hjælp af multifaktorgodkendelse (MFA)</span><span class="sxs-lookup"><span data-stu-id="cd435-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cd435-104">Den berørte bruger kan være blokeret i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="cd435-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cd435-105">Hvis det er tilfældet, vil godkendelsesforsøg for den pågældende bruger automatisk blive nægtet.</span><span class="sxs-lookup"><span data-stu-id="cd435-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cd435-106">Følg trinnene i denne artikel for at fjerne blokeringen af dem.</span><span class="sxs-lookup"><span data-stu-id="cd435-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cd435-107">Hvis fjerne blokering brugeren ikke hjalp eller brugeren ikke er blokeret, kan du prøve at nulstille MFA for brugeren, og de vil gå gennem tilmelde processen igen.</span><span class="sxs-lookup"><span data-stu-id="cd435-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cd435-108">Følg trinnene i denne artikel.</span><span class="sxs-lookup"><span data-stu-id="cd435-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cd435-109">Hvis det er første gang, du har aktiveret MFA, og dine brugere ikke kan logge ind på klienter, der ikke er browsere, såsom Outlook, Skype osv., måske er ADAL (Active Directory Authentication Library) ikke aktiveret på dit O365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="cd435-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cd435-110">I dette tilfælde skal du oprette forbindelse til Exchange Online PowerShell og køre denne cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="cd435-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>