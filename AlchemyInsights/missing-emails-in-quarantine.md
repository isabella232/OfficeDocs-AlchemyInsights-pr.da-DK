---
title: Manglende e-mails i karantæne
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569046"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="1fae3-102">Manglende e-mails i karantæne"</span><span class="sxs-lookup"><span data-stu-id="1fae3-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="1fae3-103">Administratorer kan [få vist, frigive eller slette disse meddelelser.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="1fae3-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="1fae3-104">Hvis du vil åbne Sikkerheds- & Compliance Center, skal du gå til [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="1fae3-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="1fae3-105">Hvis du vil åbne siden Karantæne direkte, skal du gå til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="1fae3-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="1fae3-106">Du kan søge efter følgende værdier:</span><span class="sxs-lookup"><span data-stu-id="1fae3-106">You can search by the following values:</span></span>  

- <span data-ttu-id="1fae3-107">**Meddelelses-id**: Meddelelsens globalt entydige id.</span><span class="sxs-lookup"><span data-stu-id="1fae3-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="1fae3-108">Hvis du vælger en meddelelse på listen, vises værdien **for meddelelses-id** i pop op-vinduet **Detaljer.**</span><span class="sxs-lookup"><span data-stu-id="1fae3-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="1fae3-109">Administratorer kan bruge [meddelelsessporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til at finde meddelelser og deres tilsvarende værdier for meddelelses-id.</span><span class="sxs-lookup"><span data-stu-id="1fae3-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="1fae3-110">**Afsenders e-mailadresse**: En enkelt afsenders e-mailadresse.</span><span class="sxs-lookup"><span data-stu-id="1fae3-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="1fae3-111">**Modtagers e-mailadresse**: En enkelt modtagers e-mailadresse.</span><span class="sxs-lookup"><span data-stu-id="1fae3-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="1fae3-112">**Emne**: Brug hele meddelelsens emne.</span><span class="sxs-lookup"><span data-stu-id="1fae3-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="1fae3-113">Der skelnes ikke mellem store og små bogstaver i søgningen.</span><span class="sxs-lookup"><span data-stu-id="1fae3-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="1fae3-114">Når du har angivet søgekriterierne, skal du klikke på ![ Knappen ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Opdater** for at filtrere resultaterne.  </span><span class="sxs-lookup"><span data-stu-id="1fae3-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="1fae3-115">De cmdletter, du bruger til at få vist og administrere meddelelser og filer i karantæne, er:</span><span class="sxs-lookup"><span data-stu-id="1fae3-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="1fae3-116">Slet-karantæneMeddelelse</span><span class="sxs-lookup"><span data-stu-id="1fae3-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="1fae3-117">Eksport-KarantæneMeddelelse</span><span class="sxs-lookup"><span data-stu-id="1fae3-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="1fae3-118">Bliv karantæneMeddelelse</span><span class="sxs-lookup"><span data-stu-id="1fae3-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="1fae3-119">[Eksempel-karantæneMeddelelse](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bemærk, at denne cmdlet kun er til meddelelser, ikke malwarefiler fra ATP til SharePoint Online, OneDrive for Business eller Teams.</span><span class="sxs-lookup"><span data-stu-id="1fae3-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="1fae3-120">Release-KarantæneMeddelelse</span><span class="sxs-lookup"><span data-stu-id="1fae3-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)