---
title: Tilbagekalde eller erstatte en e-mail-meddelelse
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353500"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="a6fa9-102">Tilbagekalde eller erstatte en e-mail-meddelelse i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a6fa9-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="a6fa9-103">Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="a6fa9-104">Hvis meddelelsen for eksempel blev sendt til en Gmail-adresse, kan du ikke tilbagekalde den.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="a6fa9-105">Du kan **kun tilbagekalde meddelelser, der er sendt fra Outlook til PC**.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="a6fa9-106">Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke tilbagekalde den.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="a6fa9-107">Som lejeradministrator kan du **tilbagekalde meddelelser på vegne af brugere ved hjælp af PowerShell** (du kan få mere at vide under: [Søg efter og slet mails](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="a6fa9-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="a6fa9-108">Du kan ikke tilbagekalde meddelelser fra administrations centeret.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="a6fa9-109">Rul ned til "Søg efter og slet mails i organisationen" for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="a6fa9-110">**Tilbagekalde eller erstatte en mail, som du har sendt**</span><span class="sxs-lookup"><span data-stu-id="a6fa9-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="a6fa9-111">I mapperuden i venstre side af Outlook-vinduet skal du vælge mappen Sendt post.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="a6fa9-112">Åbn den meddelelse, du vil tilbagekalde.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-112">Open the message that you want to recall.</span></span> <span data-ttu-id="a6fa9-113">Du skal dobbeltklikke for at åbne meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-113">You must double-click to open the message.</span></span> <span data-ttu-id="a6fa9-114">Hvis du vælger meddelelsen, så den vises i læseruden, kan du ikke tilbagekalde meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="a6fa9-115">På fanen meddelelse skal du vælge **handlinger**  >  **Tilbagekald denne meddelelse**.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="a6fa9-116">Vælg **Slet ulæste kopier af denne meddelelse** , eller **Slet ulæste kopier, og Erstat med en ny meddelelse**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="a6fa9-117">Hvis du vil sende en erstatnings meddelelse, skal du skrive meddelelsen og derefter vælge **Send**.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="a6fa9-118">Hvis en meddelelses tilbagekaldelse lykkes eller ej, afhænger af modtagernes indstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="a6fa9-119">Du kan finde flere oplysninger, herunder hvordan du kontrollerer tilbagekaldelsen, under [tilbagekald eller Erstat en mail, du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="a6fa9-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="a6fa9-120">Hvis du **_vil søge efter og slette mails i organisationen_**, er det nemmest, hvis du er Global administrator. Hvis du ikke er en global administrator, skal din konto føjes til rollegruppen eDiscovery Manager eller for rollen overholdelses Search Management.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="a6fa9-121">Hvis du vil slette meddelelser, skal du være medlem af gruppen organisations administrations rolle eller rollen søgning og sletning af administration.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="a6fa9-122">Tilladelser til disse roller tildeles i [sikkerheds & Overholdelsescenter](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a6fa9-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="a6fa9-123">[Opret en indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/content-search) for at finde den besked, der skal slettes.</span><span class="sxs-lookup"><span data-stu-id="a6fa9-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="a6fa9-124">[Opret forbindelse til sikkerheds & Compliance Center-PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a6fa9-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="a6fa9-125">Hvis du bruger MFA (multi-Factor Authentication), skal du se [oprette forbindelse til Microsoft 365 Security & Compliance Center PowerShell med multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a6fa9-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
