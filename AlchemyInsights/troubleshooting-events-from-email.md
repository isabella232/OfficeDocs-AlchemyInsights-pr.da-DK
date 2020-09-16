---
title: Fejlfinding af begivenheder fra mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658728"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="d5458-102">Fejlfinding af begivenheder fra mail</span><span class="sxs-lookup"><span data-stu-id="d5458-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="d5458-103">Kontrollér, at funktionen er aktiveret for postkassen: **Get-EventsFromEmailConfiguration- <mailbox> Identity**</span><span class="sxs-lookup"><span data-stu-id="d5458-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="d5458-104">Se derefter på "begivenheder fra mail"-logfilerne **Eksportér-MailboxDiagnosticLogs <mailbox> -komponent TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="d5458-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="d5458-105">Find den InternetMessageId, der svarer til elementet i postkassen, i "hændelser fra mail"-logfilerne.</span><span class="sxs-lookup"><span data-stu-id="d5458-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="d5458-106">TrustScore bestemmer, om elementet er tilføjet eller ej.</span><span class="sxs-lookup"><span data-stu-id="d5458-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="d5458-107">Hændelser tilføjes kun, hvis TrustScore = "betroet".</span><span class="sxs-lookup"><span data-stu-id="d5458-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="d5458-108">TrustScore bestemmes af SPF, DKIM eller dMarc egenskaber, der er i meddelelsens brevhoved.</span><span class="sxs-lookup"><span data-stu-id="d5458-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="d5458-109">Sådan får du vist disse egenskaber:</span><span class="sxs-lookup"><span data-stu-id="d5458-109">To view these properties:</span></span>

<span data-ttu-id="d5458-110">**Skrivebord Outlook**</span><span class="sxs-lookup"><span data-stu-id="d5458-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="d5458-111">Åbne elementet</span><span class="sxs-lookup"><span data-stu-id="d5458-111">Open the item</span></span>
- <span data-ttu-id="d5458-112">File-> egenskaber – > Internet brevhoveder</span><span class="sxs-lookup"><span data-stu-id="d5458-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="d5458-113">eller</span><span class="sxs-lookup"><span data-stu-id="d5458-113">or</span></span>

<span data-ttu-id="d5458-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="d5458-114">**MFCMapi**</span></span>

- <span data-ttu-id="d5458-115">Gå til elementet i indbakken</span><span class="sxs-lookup"><span data-stu-id="d5458-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="d5458-116">Søg efter PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="d5458-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="d5458-117">Disse egenskaber bestemmes og registreres under transport og routing.</span><span class="sxs-lookup"><span data-stu-id="d5458-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="d5458-118">Hvis du vil foretage yderligere fejlfinding, skal du muligvis følge med transport support om fejlene i SPF, DKIM og. DMARC.</span><span class="sxs-lookup"><span data-stu-id="d5458-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>