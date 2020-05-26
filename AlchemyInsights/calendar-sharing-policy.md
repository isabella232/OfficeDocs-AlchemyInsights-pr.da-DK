---
title: 618 Politik for kalenderdeling
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372993"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="f97d1-102">Politikfejl ved deling af en kalender</span><span class="sxs-lookup"><span data-stu-id="f97d1-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="f97d1-103">Bedød en af følgende fremgangsmåder, alt efter hvad der passer til din situation:</span><span class="sxs-lookup"><span data-stu-id="f97d1-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="f97d1-104">Opret forbindelse til Exchange Online ved hjælp af Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f97d1-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="f97d1-105">Yderligere oplysninger finder du i [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f97d1-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="f97d1-106">Åbn Exchange Management Shell på den lokale server.</span><span class="sxs-lookup"><span data-stu-id="f97d1-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="f97d1-107">Find ud af, hvilken delingspolitik brugeren har fået tildelt.</span><span class="sxs-lookup"><span data-stu-id="f97d1-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="f97d1-108">Det kan du gøre ved at køre følgende kommando og notere den returnerede politik:</span><span class="sxs-lookup"><span data-stu-id="f97d1-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="f97d1-109">Opdater delingspolitikken for brugeren.</span><span class="sxs-lookup"><span data-stu-id="f97d1-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="f97d1-110">Dette gøres ved at benytte følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="f97d1-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="f97d1-111">Åbn Exchange Administration.</span><span class="sxs-lookup"><span data-stu-id="f97d1-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="f97d1-112">Klik på **Organisation**, og dobbeltklik derefter på den politik, der er tildelt brugeren under **Individuel deling**.</span><span class="sxs-lookup"><span data-stu-id="f97d1-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="f97d1-113">Det er den politik, der blev returneret i trin 2.</span><span class="sxs-lookup"><span data-stu-id="f97d1-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="f97d1-114">Vælg det kalenderdelingsniveau, du vil tillade, under **Angiv, hvilke oplysninger du vil dele**, på siden Delingsregel. Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="f97d1-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="f97d1-115">Du kan finde flere oplysninger under: ["Politik tillader ikke tildeling af tilladelser på dette niveau til en eller flere af modtagernes)"-fejl, når brugeren forsøger at dele kalenderen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="f97d1-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
