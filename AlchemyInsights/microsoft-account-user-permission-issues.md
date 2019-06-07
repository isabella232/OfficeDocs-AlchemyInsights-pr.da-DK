---
title: Oprette og bruge en delt postkasse
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762395"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="7771b-102">Foretage fejlfinding af problemet - brugeren blev ikke fundet i mappe</span><span class="sxs-lookup"><span data-stu-id="7771b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="7771b-103">Hvis brugere får vist fejl meddelelse "bruger blev ikke fundet" i mappen.</span><span class="sxs-lookup"><span data-stu-id="7771b-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="7771b-104">Prøv igen hvor problemtypen brugeren ikke er i mappen.</span><span class="sxs-lookup"><span data-stu-id="7771b-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="7771b-105">Følgende trin kan udføres for at løse problemet.</span><span class="sxs-lookup"><span data-stu-id="7771b-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="7771b-106">Sikre, at den konto, der accepteres e-mail-invitationen er den samme konto, der bruges til at logge på senere.</span><span class="sxs-lookup"><span data-stu-id="7771b-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="7771b-107">Kontroller, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet.</span><span class="sxs-lookup"><span data-stu-id="7771b-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="7771b-108">Yderligere oplysninger finder du [hvordan du administrerer aliaser til din Microsoft-konto</a> til at administrere Office 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="7771b-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="7771b-109">Gå til hver enkelt eller flere steder, hvor brugeren modtager fejlen.</span><span class="sxs-lookup"><span data-stu-id="7771b-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="7771b-110">Føje "/ _layouts/15/people.aspx/membershipgroupid=0" (inden for de dobbelte anførselstegn) i slutningen af URL-adressen til webstedet.</span><span class="sxs-lookup"><span data-stu-id="7771b-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="7771b-111">Eksempel: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="7771b-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="7771b-112">Vælg brugeren på listen.</span><span class="sxs-lookup"><span data-stu-id="7771b-112">Select the user from the list.</span></span>

- <span data-ttu-id="7771b-113">Klik på **Fjern brugertilladelser** på båndet.</span><span class="sxs-lookup"><span data-stu-id="7771b-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="7771b-114">Tilføj brugeren igen og sende invitationen til brugeren.</span><span class="sxs-lookup"><span data-stu-id="7771b-114">Add back the User and Resend the invite to the user.</span></span>

