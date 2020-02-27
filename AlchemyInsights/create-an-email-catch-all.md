---
title: Oprette en mailfangst alle
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286103"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="5e598-102">Oprette en mailfangst alle</span><span class="sxs-lookup"><span data-stu-id="5e598-102">Create an email catch all</span></span>

<span data-ttu-id="5e598-103">Brug af en fangst alle er stærkt frarådes.</span><span class="sxs-lookup"><span data-stu-id="5e598-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="5e598-104">Det er bedre at give en hoppe tilbage til afsenderen lade afsendere vide deres budskab ikke kunne leveres som rettet, så de kan skride til handling.</span><span class="sxs-lookup"><span data-stu-id="5e598-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="5e598-105">Du kan også begrænse den overvågede postkasse til kun at fange tidligere gyldige e-mailadresser.</span><span class="sxs-lookup"><span data-stu-id="5e598-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="5e598-106">Enhver fangst alle postkasse vil modtage en hel del spam og kan i sidste ende fylde, hvis ikke nøje overvåget.</span><span class="sxs-lookup"><span data-stu-id="5e598-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="5e598-107">(Der er modtagende grænser).</span><span class="sxs-lookup"><span data-stu-id="5e598-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="5e598-108">Hvis du beslutter dig for at fortsætte, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="5e598-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="5e598-109">Opret en dynamisk distributionsgruppe & indeholde "Alle modtagertyper".</span><span class="sxs-lookup"><span data-stu-id="5e598-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="5e598-110">Opret en dedikeret postkasse for at fange mails, f.catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="5e598-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="5e598-111">Angiv DomainType til "InternalRelay" for det specifikke domæne.</span><span class="sxs-lookup"><span data-stu-id="5e598-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="5e598-112">Hvis du senere fjerner fangsten alle, skal du sørge for at indstille domænet tilbage til autoritative.</span><span class="sxs-lookup"><span data-stu-id="5e598-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="5e598-113">Opret en regel for transport af postflow på følgende måde:</span><span class="sxs-lookup"><span data-stu-id="5e598-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="5e598-114">Hvis afsenderen er "Uden for organisationen"</span><span class="sxs-lookup"><span data-stu-id="5e598-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="5e598-115">Omdiriger meddelelsen til Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="5e598-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="5e598-116">Undtagen hvis modtageren er medlem af allusers@domain.com (distributionsgruppe indeholder alle medlemmer)</span><span class="sxs-lookup"><span data-stu-id="5e598-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="5e598-117">Sørg for at validere, at nye postkasser føjes til dynamisk distributionsgruppe</span><span class="sxs-lookup"><span data-stu-id="5e598-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
