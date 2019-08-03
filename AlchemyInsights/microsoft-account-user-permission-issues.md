---
title: Foretage fejlfinding af problemet - brugeren blev ikke fundet i mappe
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249907"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="17697-102">Foretage fejlfinding af problemet - brugeren blev ikke fundet i mappe</span><span class="sxs-lookup"><span data-stu-id="17697-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="17697-103">Hvis brugere får vist fejl meddelelse "bruger blev ikke fundet" i mappen.</span><span class="sxs-lookup"><span data-stu-id="17697-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="17697-104">Prøv igen hvor problemtypen brugeren ikke er i mappen.</span><span class="sxs-lookup"><span data-stu-id="17697-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="17697-105">Følgende trin kan udføres for at løse problemet.</span><span class="sxs-lookup"><span data-stu-id="17697-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="17697-106">Sikre, at den konto, der accepteres e-mail-invitationen er den samme konto, der bruges til at logge på senere.</span><span class="sxs-lookup"><span data-stu-id="17697-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="17697-107">Kontroller, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet.</span><span class="sxs-lookup"><span data-stu-id="17697-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="17697-108">Yderligere oplysninger finder du [hvordan du administrerer aliaser til din Microsoft-konto</a> til at administrere Office 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="17697-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="17697-109">Gå til hver enkelt eller flere steder, hvor brugeren modtager fejlen.</span><span class="sxs-lookup"><span data-stu-id="17697-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="17697-110">Føje "/ _layouts/15/people.aspx/membershipgroupid=0" (inden for de dobbelte anførselstegn) i slutningen af URL-adressen til webstedet.</span><span class="sxs-lookup"><span data-stu-id="17697-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="17697-111">Eksempel: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="17697-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="17697-112">Vælg brugeren på listen.</span><span class="sxs-lookup"><span data-stu-id="17697-112">Select the user from the list.</span></span>

- <span data-ttu-id="17697-113">Klik på **Fjern brugertilladelser** på båndet.</span><span class="sxs-lookup"><span data-stu-id="17697-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="17697-114">Tilføj brugeren igen og sende invitationen til brugeren.</span><span class="sxs-lookup"><span data-stu-id="17697-114">Add back the User and Resend the invite to the user.</span></span>

