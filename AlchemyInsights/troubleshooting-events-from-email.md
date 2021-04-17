---
title: Fejlfinding af hændelser fra mail
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834833"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="cfb5a-102">Fejlfinding af hændelser fra mail</span><span class="sxs-lookup"><span data-stu-id="cfb5a-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="cfb5a-103">Bekræft, at funktionen er aktiveret for **postkassen: Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="cfb5a-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="cfb5a-104">Kig derefter på "Begivenheder fra **mail"-logfilerne Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="cfb5a-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="cfb5a-105">I logfilerne "Begivenheder fra mail" skal du finde det InternetMessageId, der svarer til elementet i postkassen.</span><span class="sxs-lookup"><span data-stu-id="cfb5a-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="cfb5a-106">TrustScore bestemmer, om elementet tilføjes eller ej.</span><span class="sxs-lookup"><span data-stu-id="cfb5a-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="cfb5a-107">Hændelser tilføjes kun, hvis TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="cfb5a-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="cfb5a-108">TrustScore bestemmes af SPF-, Dkim- eller Dmarc-egenskaberne, som findes i brevhovedet.</span><span class="sxs-lookup"><span data-stu-id="cfb5a-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="cfb5a-109">Sådan får du vist disse egenskaber:</span><span class="sxs-lookup"><span data-stu-id="cfb5a-109">To view these properties:</span></span>

<span data-ttu-id="cfb5a-110">**Skrivebordsversionen af Outlook**</span><span class="sxs-lookup"><span data-stu-id="cfb5a-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="cfb5a-111">Åbne elementet</span><span class="sxs-lookup"><span data-stu-id="cfb5a-111">Open the item</span></span>
- <span data-ttu-id="cfb5a-112">Egenskaber for filer > -> internetoverskrifter</span><span class="sxs-lookup"><span data-stu-id="cfb5a-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="cfb5a-113">eller</span><span class="sxs-lookup"><span data-stu-id="cfb5a-113">or</span></span>

<span data-ttu-id="cfb5a-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="cfb5a-114">**MFCMapi**</span></span>

- <span data-ttu-id="cfb5a-115">Gå til elementet i indbakken</span><span class="sxs-lookup"><span data-stu-id="cfb5a-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="cfb5a-116">Se efter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="cfb5a-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="cfb5a-117">Disse egenskaber bestemmes og registreres under transport og routing.</span><span class="sxs-lookup"><span data-stu-id="cfb5a-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="cfb5a-118">For yderligere fejlfinding kan det være nødvendigt at følge op med Transport Support vedrørende fejl i SPF, DKIM og.eller DMARC.</span><span class="sxs-lookup"><span data-stu-id="cfb5a-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>