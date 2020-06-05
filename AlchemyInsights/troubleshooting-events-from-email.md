---
title: Fejlfinding af hændelser fra mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569007"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="428da-102">Fejlfinding af hændelser fra mail</span><span class="sxs-lookup"><span data-stu-id="428da-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="428da-103">Kontroller, at funktionen er aktiveret for postkassen: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="428da-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="428da-104">Så kig på 'Begivenheder fra e-mail' logger **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="428da-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="428da-105">Find det InternetMessageId, der svarer til elementet i postkassen, i logfilerne 'Hændelser fra e-mail'.</span><span class="sxs-lookup"><span data-stu-id="428da-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="428da-106">TrustScore bestemmer, om varen tilføjes eller ej.</span><span class="sxs-lookup"><span data-stu-id="428da-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="428da-107">Hændelser tilføjes kun, hvis TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="428da-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="428da-108">TrustScore bestemmes af egenskaberne SPF, Dkim eller Dmarc, som findes i brevhovedet.</span><span class="sxs-lookup"><span data-stu-id="428da-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="428da-109">Sådan får du vist disse egenskaber:</span><span class="sxs-lookup"><span data-stu-id="428da-109">To view these properties:</span></span>

<span data-ttu-id="428da-110">**Outlook på computeren**</span><span class="sxs-lookup"><span data-stu-id="428da-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="428da-111">Åbne elementet</span><span class="sxs-lookup"><span data-stu-id="428da-111">Open the item</span></span>
- <span data-ttu-id="428da-112">Egenskaber for fil -> -> Internetheads</span><span class="sxs-lookup"><span data-stu-id="428da-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="428da-113">Eller</span><span class="sxs-lookup"><span data-stu-id="428da-113">or</span></span>

<span data-ttu-id="428da-114">**MFCMapi delte et eller flere**</span><span class="sxs-lookup"><span data-stu-id="428da-114">**MFCMapi**</span></span>

- <span data-ttu-id="428da-115">Gå til elementet i indbakken</span><span class="sxs-lookup"><span data-stu-id="428da-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="428da-116">Kig efter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="428da-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="428da-117">Disse egenskaber bestemmes og registreres under transport og ruteføring.</span><span class="sxs-lookup"><span data-stu-id="428da-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="428da-118">For yderligere fejlfinding kan det være nødvendigt at følge op med Transport Support om fejl i SPF, DKIM og.eller DMARC.</span><span class="sxs-lookup"><span data-stu-id="428da-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>