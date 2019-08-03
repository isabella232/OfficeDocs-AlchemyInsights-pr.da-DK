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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250159"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="53c5f-102">Problemer med MFA</span><span class="sxs-lookup"><span data-stu-id="53c5f-102">Issues with MFA</span></span>
<span data-ttu-id="53c5f-103">Der er et par ting, hvis brugere ikke logge på ved hjælp af godkendelse i flere niveauer (MFA)</span><span class="sxs-lookup"><span data-stu-id="53c5f-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="53c5f-104">Den pågældende bruger være blokeret i Azure Active Directory-Portal.</span><span class="sxs-lookup"><span data-stu-id="53c5f-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="53c5f-105">Hvis det er tilfældet, forsøger godkendelse for den pågældende specifikke bruger automatisk nægtes.</span><span class="sxs-lookup"><span data-stu-id="53c5f-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="53c5f-106">Følg trinnene i denne artikel for at fjerne blokeringen af dem.</span><span class="sxs-lookup"><span data-stu-id="53c5f-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="53c5f-107">Hvis brugeren ikke er blokeret, eller fjerne blokeringen af brugeren ikke kunne hjælpe kan du prøve at nulstille MFA for brugeren, og de vil gå gennem Registrer igen.</span><span class="sxs-lookup"><span data-stu-id="53c5f-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="53c5f-108">Følg trinnene i denne artikel.</span><span class="sxs-lookup"><span data-stu-id="53c5f-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="53c5f-109">Hvis det er første gang, du aktiverede MFA og dine brugere kan ikke logge på andre browsere end klienter som Outlook, Skype osv, er måske ADAL (Active Directory-godkendelse bibliotek) ikke aktiveret på dit abonnement på O365.</span><span class="sxs-lookup"><span data-stu-id="53c5f-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="53c5f-110">I dette tilfælde skal du oprette forbindelse til Exchange Online Powershell og køre denne cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="53c5f-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>