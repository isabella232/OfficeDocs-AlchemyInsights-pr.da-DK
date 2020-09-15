---
title: Oprette en e-mail-samling
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712980"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="c4e1c-102">Oprette en e-mail-samling</span><span class="sxs-lookup"><span data-stu-id="c4e1c-102">Create an email catch all</span></span>

<span data-ttu-id="c4e1c-103">Brug af en catch all er stærkt frarådet.</span><span class="sxs-lookup"><span data-stu-id="c4e1c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="c4e1c-104">Det er bedre at stille tilbage til afsenderen besked om, at afsenderen ved, at deres meddelelse ikke blev leveret som løst, så de kan handle.</span><span class="sxs-lookup"><span data-stu-id="c4e1c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="c4e1c-105">Du kan også begrænse den overvågede postkasse til kun at fange tidligere gyldige mailadresser.</span><span class="sxs-lookup"><span data-stu-id="c4e1c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="c4e1c-106">Alle catch-alle postkasser modtager en god slags spam og kan til enhver udfyldnings besked se ud, hvis den ikke er tæt overvåget.</span><span class="sxs-lookup"><span data-stu-id="c4e1c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="c4e1c-107">Der er grænser for modtagelse.</span><span class="sxs-lookup"><span data-stu-id="c4e1c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="c4e1c-108">Hvis du beslutter dig for at fortsætte, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="c4e1c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="c4e1c-109">Opret en dynamisk distributionsgruppe & du medtage "alle modtagertyper".</span><span class="sxs-lookup"><span data-stu-id="c4e1c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="c4e1c-110">Opret en dedikeret postkasse til at fange mails, f. eks catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="c4e1c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="c4e1c-111">For det specifikke domæne skal du angive DomainType til "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="c4e1c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="c4e1c-112">Hvis du senere fjerner catch all, skal du sørge for at indstille domænet tilbage til autoritativ.</span><span class="sxs-lookup"><span data-stu-id="c4e1c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="c4e1c-113">Opret en fejlfinding mailflowhttps://Configure.Office.com/scenario.aspx?SID=12-transport regel på følgende måde:</span><span class="sxs-lookup"><span data-stu-id="c4e1c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="c4e1c-114">Hvis afsenderen er "uden for organisationen"</span><span class="sxs-lookup"><span data-stu-id="c4e1c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="c4e1c-115">Omdiriger meddelelsen til Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="c4e1c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="c4e1c-116">Undtagen, hvis modtageren er medlem af allusers@domain.com (distributionsgruppe indeholder alle medlemmer)</span><span class="sxs-lookup"><span data-stu-id="c4e1c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="c4e1c-117">Sørg for at bekræfte, at nye postkasser føjes til den dynamiske distributionsgruppe</span><span class="sxs-lookup"><span data-stu-id="c4e1c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
