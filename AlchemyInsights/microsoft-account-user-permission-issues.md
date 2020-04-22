---
title: Fejlfindingsproblem - Brugeren blev ikke fundet i mappen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702732"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="77a39-102">Fejlfindingsproblem - Brugeren blev ikke fundet i mappen</span><span class="sxs-lookup"><span data-stu-id="77a39-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="77a39-103">Hvis brugerne modtager fejlmeddelelsen "Brugeren kan ikke findes" i mappen, skal du prøve igen, hvor problemtypen er Bruger, der ikke er i mappen.</span><span class="sxs-lookup"><span data-stu-id="77a39-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="77a39-104">Følgende trin kan udføres for at foretage fejlfinding af problemet.</span><span class="sxs-lookup"><span data-stu-id="77a39-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="77a39-105">Sørg for, at den konto, der har accepteret e-mailinvitationen, er den samme konto, som bruges til at logge på senere.</span><span class="sxs-lookup"><span data-stu-id="77a39-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="77a39-106">Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet.</span><span class="sxs-lookup"><span data-stu-id="77a39-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="77a39-107">Du kan finde flere oplysninger under [Sådan</a> administrerer du aliasser for din Microsoft-konto for at administrere Microsoft 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="77a39-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="77a39-108">Find hvert eller flere websteder, hvor brugeren modtager fejlen.</span><span class="sxs-lookup"><span data-stu-id="77a39-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="77a39-109">Føj "/_layouts/15/people.aspx/membershipgroupid=0" (inden for dobbelttilbud) til slutningen af webstedets URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="77a39-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="77a39-110">Eksempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="77a39-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="77a39-111">Vælg brugeren på listen.</span><span class="sxs-lookup"><span data-stu-id="77a39-111">Select the user from the list.</span></span>

- <span data-ttu-id="77a39-112">Klik på **Fjern brugertilladelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="77a39-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="77a39-113">Tilføj invitationen tilbage, og send invitationen til brugeren igen.</span><span class="sxs-lookup"><span data-stu-id="77a39-113">Add back the User and Resend the invite to the user.</span></span>

