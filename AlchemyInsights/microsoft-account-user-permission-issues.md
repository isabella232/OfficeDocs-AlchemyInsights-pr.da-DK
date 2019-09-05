---
title: Fejlfinding af problem-brugeren blev ikke fundet i mappen
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754186"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ae19c-102">Fejlfinding af problem-brugeren blev ikke fundet i mappen</span><span class="sxs-lookup"><span data-stu-id="ae19c-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ae19c-103">Selv om brugernes er modtager fejl besked "bruger kan ikke ' være oprette" i den bibliotek.</span><span class="sxs-lookup"><span data-stu-id="ae19c-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="ae19c-104">Prøv igen, hvor problemtypen er bruger ikke i mappen.</span><span class="sxs-lookup"><span data-stu-id="ae19c-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ae19c-105">Følgende trin kan udføres for at løse problemet.</span><span class="sxs-lookup"><span data-stu-id="ae19c-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ae19c-106">Sørg for, at den konto, der accepterede e-mailinvitationen, er den samme konto, som bruges til at logge på senere.</span><span class="sxs-lookup"><span data-stu-id="ae19c-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ae19c-107">Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet.</span><span class="sxs-lookup"><span data-stu-id="ae19c-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ae19c-108">Du kan finde flere oplysninger under [Sådan administrerer du aliasser for din</a> Microsoft-konto for at administrere Office 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ae19c-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ae19c-109">Gå til hvert sted (er), hvor brugeren modtager fejlen.</span><span class="sxs-lookup"><span data-stu-id="ae19c-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ae19c-110">Tilføj "/_layouts/15/People.aspx/membershipgroupid = 0" (i dobbelt anførselstegn) til slutningen af webstedets URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="ae19c-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ae19c-111">Eksempel: https:/_Lt_ "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="ae19c-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ae19c-112">Vælg brugeren på listen.</span><span class="sxs-lookup"><span data-stu-id="ae19c-112">Select the user from the list.</span></span>

- <span data-ttu-id="ae19c-113">Klik på **Fjern brugertilladelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="ae19c-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ae19c-114">Tilføj brugeren tilbage, og send invitationen til brugeren igen.</span><span class="sxs-lookup"><span data-stu-id="ae19c-114">Add back the User and Resend the invite to the user.</span></span>

