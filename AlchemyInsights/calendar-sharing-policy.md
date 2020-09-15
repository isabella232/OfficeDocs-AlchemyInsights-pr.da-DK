---
title: 618 kalender delings politik
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684224"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="01a72-102">Politik fejl ved deling af en kalender</span><span class="sxs-lookup"><span data-stu-id="01a72-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="01a72-103">Gør et af følgende, afhængigt af din situation:</span><span class="sxs-lookup"><span data-stu-id="01a72-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="01a72-104">Opret forbindelse til Exchange Online ved hjælp af Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="01a72-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="01a72-105">Hvis du vil have mere at vide, skal du se [oprette forbindelse til Exchange Online ved hjælp af Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="01a72-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="01a72-106">Åbn Exchange Management Shell på den lokale server.</span><span class="sxs-lookup"><span data-stu-id="01a72-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="01a72-107">Find ud af, hvilken delings politik der er tildelt brugeren.</span><span class="sxs-lookup"><span data-stu-id="01a72-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="01a72-108">Hvis du vil gøre dette, skal du køre følgende kommando og bemærke, at den returnerede politik:</span><span class="sxs-lookup"><span data-stu-id="01a72-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="01a72-109">Opdater delings politikken for brugeren.</span><span class="sxs-lookup"><span data-stu-id="01a72-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="01a72-110">Dette gøres ved at benytte følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="01a72-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="01a72-111">Åbn Exchange administration.</span><span class="sxs-lookup"><span data-stu-id="01a72-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="01a72-112">Klik på **organisation**, og dobbeltklik derefter på den politik, der er tildelt brugeren under **individuel deling**.</span><span class="sxs-lookup"><span data-stu-id="01a72-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="01a72-113">Dette er den politik, der blev returneret i trin 2.</span><span class="sxs-lookup"><span data-stu-id="01a72-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="01a72-114">På siden delings regel skal du vælge det niveau for kalender deling, du vil tillade under **angive, hvilke oplysninger du vil dele**. Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="01a72-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="01a72-115">Du kan finde flere oplysninger under: ["politikken tillader ikke, at der tildeles tilladelser på dette niveau til en eller flere af modtager meddelelsen", når brugeren forsøger at dele kalender](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="01a72-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
