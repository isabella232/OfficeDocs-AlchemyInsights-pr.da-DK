---
title: Opret en mail, opfang alle
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816194"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="b2273-102">Opret en mail, opfang alle</span><span class="sxs-lookup"><span data-stu-id="b2273-102">Create an email catch all</span></span>

<span data-ttu-id="b2273-103">Det frarådes på det kraftigste at bruge en opfangne.</span><span class="sxs-lookup"><span data-stu-id="b2273-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="b2273-104">Det er bedre at give afsenderen en tilbagevisning, så afsenderen ved, at meddelelsen ikke kunne leveres som adresseret, så afsenderen kan handle.</span><span class="sxs-lookup"><span data-stu-id="b2273-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="b2273-105">Du kan også begrænse den overvågede postkasse til kun at fange tidligere gyldige mailadresser.</span><span class="sxs-lookup"><span data-stu-id="b2273-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="b2273-106">Enhver opfang alle postkasser modtager en hel del spam og kan blive fyldt op med tiden, hvis de ikke overvåges nøje.</span><span class="sxs-lookup"><span data-stu-id="b2273-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="b2273-107">(Der modtager begrænsninger).</span><span class="sxs-lookup"><span data-stu-id="b2273-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="b2273-108">Hvis du beslutter dig for at fortsætte, skal du følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="b2273-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="b2273-109">Opret en dynamisk distributionsgruppe, & inkluderer "Alle modtagertyper".</span><span class="sxs-lookup"><span data-stu-id="b2273-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="b2273-110">Opret en dedikeret postkasse for at få mails, f.eks. catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="b2273-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="b2273-111">For det specifikke domæne skal du indstille DomainType til "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="b2273-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="b2273-112">Hvis du senere fjerner alle uønskede, skal du sørge for at indstille domænet tilbage til Autoritativ.</span><span class="sxs-lookup"><span data-stu-id="b2273-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="b2273-113">Opret en transportregel for mailflow på følgende måde:</span><span class="sxs-lookup"><span data-stu-id="b2273-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="b2273-114">Hvis afsenderen er "Uden for organisationen"</span><span class="sxs-lookup"><span data-stu-id="b2273-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="b2273-115">Omdiriger meddelelsen til Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="b2273-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="b2273-116">Undtagen hvis modtageren er medlem af allusers@domain.com (Distributionsgruppe indeholder alle medlemmer)</span><span class="sxs-lookup"><span data-stu-id="b2273-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="b2273-117">Sørg for at validere, at nye postkasser føjes til den dynamiske distributionsgruppe</span><span class="sxs-lookup"><span data-stu-id="b2273-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
