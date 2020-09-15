---
title: Manglende mails i karantæne
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673708"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="86352-102">Manglende mails i karantæne</span><span class="sxs-lookup"><span data-stu-id="86352-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="86352-103">Administratorer kan [få vist, udgive eller slette disse meddelelser.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="86352-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="86352-104">Hvis du vil åbne sikkerheds & overholdelses Center, skal du gå til [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="86352-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="86352-105">Gå til for at åbne siden karantæne direkte [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="86352-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="86352-106">Du kan søge efterfølgende værdier:</span><span class="sxs-lookup"><span data-stu-id="86352-106">You can search by the following values:</span></span>  

- <span data-ttu-id="86352-107">**Meddelelses-id**: meddelelsens globalt entydige id.</span><span class="sxs-lookup"><span data-stu-id="86352-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="86352-108">Hvis du vælger en meddelelse på listen, vises  **meddelelses-ID-**  værdien i pop op-ruden med  **detaljer**  , der vises.</span><span class="sxs-lookup"><span data-stu-id="86352-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="86352-109">Administratorer kan bruge [meddelelsessporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til at finde meddelelser og deres tilsvarende meddelelses-id-værdier.</span><span class="sxs-lookup"><span data-stu-id="86352-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="86352-110">**Afsender mailadresse**: en enkelt afsenders mailadresse.</span><span class="sxs-lookup"><span data-stu-id="86352-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="86352-111">**Modtager mailadresse**: en enkelt modtagers mailadresse.</span><span class="sxs-lookup"><span data-stu-id="86352-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="86352-112">**Emne**: Brug hele meddelelsens emne.</span><span class="sxs-lookup"><span data-stu-id="86352-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="86352-113">Søgningen skelner ikke mellem store og små bogstaver.</span><span class="sxs-lookup"><span data-stu-id="86352-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="86352-114">Når du har angivet søgekriterierne, skal du klikke på Opdater ![ knap ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** for at filtrere resultaterne.  </span><span class="sxs-lookup"><span data-stu-id="86352-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="86352-115">De cmdletter, du bruger til at få vist og administrere meddelelser og filer i karantæne, er:</span><span class="sxs-lookup"><span data-stu-id="86352-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="86352-116">Slet-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86352-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="86352-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86352-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="86352-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86352-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="86352-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bemærk, at denne cmdlet kun gælder for meddelelser, ikke malware-filer fra DTT til SharePoint Online, OneDrive for Business eller teams.</span><span class="sxs-lookup"><span data-stu-id="86352-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="86352-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="86352-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)