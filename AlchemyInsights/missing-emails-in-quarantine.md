---
title: Manglende mails i karantæne
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
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539818"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="74ae6-102">Manglende mails i karantæne"</span><span class="sxs-lookup"><span data-stu-id="74ae6-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="74ae6-103">Administratorer kan [få vist, slippe eller slette disse meddelelser.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="74ae6-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="74ae6-104">Hvis du vil åbne Security & Compliance Center, skal du gå til [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="74ae6-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="74ae6-105">Hvis du vil åbne siden Karantæne direkte, skal du gå til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="74ae6-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="74ae6-106">Du kan søge efter følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="74ae6-106">You can search by the following values:</span></span>  

- <span data-ttu-id="74ae6-107">**Meddelelses-id:** GUID (Globally Unique Identifier) i meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="74ae6-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="74ae6-108">Hvis du vælger en meddelelse på listen, vises værdien  **Meddelelses-id**  i pop  **op-ruden**  Detaljer, der vises.</span><span class="sxs-lookup"><span data-stu-id="74ae6-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="74ae6-109">Administratorer kan bruge [meddelelsessporing til](/microsoft-365/security/office-365-security/message-trace-scc) at finde meddelelser og deres tilsvarende meddelelses-id-værdier.</span><span class="sxs-lookup"><span data-stu-id="74ae6-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="74ae6-110">**Afsendermailadresse:** En enkelt afsenders mailadresse.</span><span class="sxs-lookup"><span data-stu-id="74ae6-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="74ae6-111">**Modtagermailadresse:** En enkelt modtagers mailadresse.</span><span class="sxs-lookup"><span data-stu-id="74ae6-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="74ae6-112">**Emne:** Brug hele meddelelsens emne.</span><span class="sxs-lookup"><span data-stu-id="74ae6-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="74ae6-113">Der er ikke store og små bogstaver i søgningen.</span><span class="sxs-lookup"><span data-stu-id="74ae6-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="74ae6-114">Når du har angivet søgekriterierne, skal du klikke på ![ Opdater knap ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Opdater** for at filtrere resultaterne.</span><span class="sxs-lookup"><span data-stu-id="74ae6-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="74ae6-115">De cmdlet'er, du bruger til at få vist og administrere meddelelser og filer i karantæne, er:</span><span class="sxs-lookup"><span data-stu-id="74ae6-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="74ae6-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="74ae6-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="74ae6-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="74ae6-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="74ae6-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="74ae6-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="74ae6-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Bemærk, at denne cmdlet kun er til meddelelser, ikke malwarefiler fra Microsoft Defender til Office 365 til SharePoint Online, OneDrive for Business eller Teams.</span><span class="sxs-lookup"><span data-stu-id="74ae6-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="74ae6-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="74ae6-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)