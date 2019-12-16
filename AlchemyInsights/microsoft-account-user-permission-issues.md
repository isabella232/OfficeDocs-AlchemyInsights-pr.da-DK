---
title: Fejlfinding af problem-brugeren blev ikke fundet i mappen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054804"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="eeae7-102">Fejlfinding af problem-brugeren blev ikke fundet i mappen</span><span class="sxs-lookup"><span data-stu-id="eeae7-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="eeae7-103">Hvis brugerne får fejlmeddelelsen "brugeren kan ikke findes" i mappen, skal du prøve igen, hvor problemtypen er bruger ikke i mappen.</span><span class="sxs-lookup"><span data-stu-id="eeae7-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="eeae7-104">Følgende trin kan udføres for at løse problemet.</span><span class="sxs-lookup"><span data-stu-id="eeae7-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="eeae7-105">Sørg for, at den konto, der accepterede e-mailinvitationen, er den samme konto, som bruges til at logge på senere.</span><span class="sxs-lookup"><span data-stu-id="eeae7-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="eeae7-106">Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet.</span><span class="sxs-lookup"><span data-stu-id="eeae7-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="eeae7-107">Du kan finde flere oplysninger under [Sådan administrerer du aliasser for din</a> Microsoft-konto for at administrere Office 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="eeae7-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="eeae7-108">Gå til hvert sted (er), hvor brugeren modtager fejlen.</span><span class="sxs-lookup"><span data-stu-id="eeae7-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="eeae7-109">Tilføj "/_layouts/15/People.aspx/membershipgroupid = 0" (i dobbelt anførselstegn) til slutningen af webstedets webadresse.</span><span class="sxs-lookup"><span data-stu-id="eeae7-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="eeae7-110">Eksempel: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="eeae7-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="eeae7-111">Vælg brugeren på listen.</span><span class="sxs-lookup"><span data-stu-id="eeae7-111">Select the user from the list.</span></span>

- <span data-ttu-id="eeae7-112">Klik på **Fjern brugertilladelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="eeae7-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="eeae7-113">Tilføj brugeren tilbage, og send invitationen til brugeren igen.</span><span class="sxs-lookup"><span data-stu-id="eeae7-113">Add back the User and Resend the invite to the user.</span></span>

