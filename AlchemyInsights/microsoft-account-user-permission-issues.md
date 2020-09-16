---
title: Fejlfinding af problem – brugeren blev ikke fundet i katalog
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725401"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6ce0b-102">Fejlfinding af problem – brugeren blev ikke fundet i katalog</span><span class="sxs-lookup"><span data-stu-id="6ce0b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6ce0b-103">Hvis brugerne får vist fejlmeddelelsen "brugeren blev ikke fundet" i adresselisten, skal du prøve igen, hvor problemtypen ikke er på adresselisten.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6ce0b-104">Følgende trin kan udføres for at foretage fejlfinding af problemet.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6ce0b-105">Kontrollér, at den konto, der accepterede e-mail-invitationen, er den samme konto, der bruges til at logge på senere.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6ce0b-106">Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6ce0b-107">Hvis du vil have mere at vide, skal du se [Sådan administreres aliasser for din Microsoft-konto </a> til at administrere Microsoft 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="6ce0b-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6ce0b-108">Gå til hvert websted (e), hvor brugeren modtager fejlen.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6ce0b-109">Tilføj "/_layouts/15/People.aspx/membershipgroupid = 0" (inden for dobbelte anførselstegn) i slutningen af webstedets URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6ce0b-110">Eksempel: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6ce0b-111">Vælg brugeren på listen.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-111">Select the user from the list.</span></span>

- <span data-ttu-id="6ce0b-112">Klik på **Fjern brugertilladelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6ce0b-113">Tilføj brugeren tilbage og send invitationen til brugeren igen.</span><span class="sxs-lookup"><span data-stu-id="6ce0b-113">Add back the User and Resend the invite to the user.</span></span>

