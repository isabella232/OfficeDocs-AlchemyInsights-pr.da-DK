---
title: Outlook-skrivebordet tilbagekaldelse eller Erstat en mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496105"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="aed2f-102">Tilbagekalde eller erstatte en Outlook-mail</span><span class="sxs-lookup"><span data-stu-id="aed2f-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="aed2f-103">Som administrator kan du **tilbagekalde meddelelser på vegne af brugere, som bruger PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="aed2f-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="aed2f-104">Du kan ikke tilbagekalde meddelelser fra administrationscenteret.</span><span class="sxs-lookup"><span data-stu-id="aed2f-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="aed2f-105">Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="aed2f-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="aed2f-106">Hvis beskeden blev sendt til en Gmail-adresse, kan du for eksempel ikke huske den.</span><span class="sxs-lookup"><span data-stu-id="aed2f-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="aed2f-107">Du kan **kun tilbagekalde meddelelser, som er sendt fra Outlook 2016 på pc'en**.</span><span class="sxs-lookup"><span data-stu-id="aed2f-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="aed2f-108">Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke huske den.</span><span class="sxs-lookup"><span data-stu-id="aed2f-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="aed2f-109">Sådan tilbagekaldes eller erstattes en mail:</span><span class="sxs-lookup"><span data-stu-id="aed2f-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="aed2f-110">Vælg mappen Sendt post i mapperuden til venstre i Outlook-vinduet.</span><span class="sxs-lookup"><span data-stu-id="aed2f-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="aed2f-111">Dobbeltklik på den meddelelse, du vil tilbagekalde, for at åbne den.</span><span class="sxs-lookup"><span data-stu-id="aed2f-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="aed2f-112">Vælg fanen **meddelelse** , og vælg derefter **handlinger** > **Tilbagekald denne meddelelse**.</span><span class="sxs-lookup"><span data-stu-id="aed2f-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="aed2f-113">Vælg **Slet ulæste kopier af denne meddelelse** , eller **Slet ulæste kopier, og Erstat med en ny meddelelse**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="aed2f-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="aed2f-114">Hvis du sender en erstatnings meddelelse, skal du skrive meddelelsen og derefter vælge **Send**.</span><span class="sxs-lookup"><span data-stu-id="aed2f-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="aed2f-115">Succesen eller fiaskoen for en meddelelse tilbagekaldelse afhænger af modtagerens indstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="aed2f-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="aed2f-116">Se [denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)for at få trin til at kontrollere tilbagekaldelsen.</span><span class="sxs-lookup"><span data-stu-id="aed2f-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="aed2f-117">Søg efter og slet e-mail-meddelelser i din organisation</span><span class="sxs-lookup"><span data-stu-id="aed2f-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="aed2f-118">Hvis du ikke er Global administrator, skal din konto føjes til rollen eDiscovery Manager eller styring af Overholdelsessøgning for at søge efter meddelelser.</span><span class="sxs-lookup"><span data-stu-id="aed2f-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="aed2f-119">Hvis du vil slette meddelelser, skal du tilmelde dig organisations administrations rollegruppen eller rollen Søg og fjernadministration.</span><span class="sxs-lookup"><span data-stu-id="aed2f-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="aed2f-120">Tilladelserne til disse roller tildeles i [Security and Compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="aed2f-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="aed2f-121">[Opret en indholdssøgning](https://docs.microsoft.com/office365/securitycompliance/content-search) for at finde den meddelelse, der skal slettes.</span><span class="sxs-lookup"><span data-stu-id="aed2f-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="aed2f-122">[Opret forbindelse til Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="aed2f-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="aed2f-123">Hvis du bruger multifaktorgodkendelse, kan du se under [Opret forbindelse til Office 365 Security and Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="aed2f-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>