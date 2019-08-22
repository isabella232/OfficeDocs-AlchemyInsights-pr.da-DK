---
title: Outlook stationære tilbagekaldelse eller erstatte en e-mail-meddelelse
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496105"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="fc37d-102">Tilbagekalde eller erstatte en e-mail i Outlook</span><span class="sxs-lookup"><span data-stu-id="fc37d-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="fc37d-103">Som administrator kan du **tilbagekaldelse af meddelelser på vegne af brugere ved hjælp af PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="fc37d-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="fc37d-104">Du kan ikke trække meddelelser fra admin center.</span><span class="sxs-lookup"><span data-stu-id="fc37d-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="fc37d-105">Du kan **kun tilbagekaldelse af meddelelser, der sendes til personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="fc37d-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="fc37d-106">Hvis meddelelsen blev sendt til en Gmail-adresse, for eksempel, ikke kan du huske den.</span><span class="sxs-lookup"><span data-stu-id="fc37d-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="fc37d-107">Du kan **kun tilbagekaldelsesmeddelelsen, der sendes fra Outlook 2016 på PC'EN**.</span><span class="sxs-lookup"><span data-stu-id="fc37d-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="fc37d-108">Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på World Wide web, kan du trække den tilbage.</span><span class="sxs-lookup"><span data-stu-id="fc37d-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="fc37d-109">Du tilbagekalder eller erstatter en e-mail-meddelelse:</span><span class="sxs-lookup"><span data-stu-id="fc37d-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="fc37d-110">Vælg mappen Sendt post i mapperuden i Outlook-vinduet til venstre.</span><span class="sxs-lookup"><span data-stu-id="fc37d-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="fc37d-111">Dobbeltklik på den meddelelse, du vil tilbagekalde for at åbne den.</span><span class="sxs-lookup"><span data-stu-id="fc37d-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="fc37d-112">Vælg fanen **meddelelse** og derefter vælge **Handlinger** > **Tilbagekald denne meddelelse**.</span><span class="sxs-lookup"><span data-stu-id="fc37d-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="fc37d-113">Vælg **Slette ulæste kopier af denne meddelelse** eller **Slette ulæste kopier og erstatte med en ny meddelelse**, og klik derefter på **OK**.</span><span class="sxs-lookup"><span data-stu-id="fc37d-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="fc37d-114">Hvis du sender en meddelelse til udskiftning, Skriv meddelelsen, og vælg derefter **Send**.</span><span class="sxs-lookup"><span data-stu-id="fc37d-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="fc37d-115">Lykkes eller ej af en tilbagekaldelse af meddelelse afhænger af modtagerens indstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="fc37d-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="fc37d-116">Hvordan at kontrollere tilbagekaldelsen, finder du [i denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="fc37d-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="fc37d-117">Søge efter og slette e-mail-meddelelser i din organisation</span><span class="sxs-lookup"><span data-stu-id="fc37d-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="fc37d-118">Hvis du ikke er en global administrator, skal kontoen føjes til eDiscovery lederrolle eller rollen overholdelse søgning til at søge efter meddelelser.</span><span class="sxs-lookup"><span data-stu-id="fc37d-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="fc37d-119">Hvis du vil slette meddelelser, skal du deltage i rollegruppe organisationsstyring eller rollen søgning og Rens.</span><span class="sxs-lookup"><span data-stu-id="fc37d-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="fc37d-120">Der tildeles tilladelser til disse roller i [center for sikkerhed og kompatibilitet](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="fc37d-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="fc37d-121">[Opret et indhold søge](https://docs.microsoft.com/office365/securitycompliance/content-search) at finde meddelelsen slettes.</span><span class="sxs-lookup"><span data-stu-id="fc37d-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="fc37d-122">[Oprette forbindelse til sikkerhed og PowerShell Overholdelsescenter](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="fc37d-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="fc37d-123">Hvis du bruger godkendelse i flere niveauer, kan du se [Opret forbindelse til Office 365 sikkerhed og kompatibilitet Center PowerShell ved hjælp af godkendelse i flere niveauer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="fc37d-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>