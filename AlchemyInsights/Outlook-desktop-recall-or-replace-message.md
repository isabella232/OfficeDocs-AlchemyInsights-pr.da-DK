---
title: Tilbagekald af Outlook på skrivebordet, eller Erstat en mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663984"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="0b3e8-102">Tilbagekalde eller erstatte en Outlook-mail</span><span class="sxs-lookup"><span data-stu-id="0b3e8-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="0b3e8-103">Som administrator kan du **tilbagekalde meddelelser på vegne af brugere ved hjælp af PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="0b3e8-104">Du kan ikke tilbagekalde meddelelser fra administrations centeret.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="0b3e8-105">Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="0b3e8-106">Hvis meddelelsen blev sendt til en Gmail-adresse, kan du for eksempel ikke tilbagekalde den.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="0b3e8-107">Du kan **kun tilbagekalde meddelelser, der er sendt fra Outlook 2016 på pc'en**.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="0b3e8-108">Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke tilbagekalde den.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="0b3e8-109">Sådan tilbagekaldes eller erstattes en mail:</span><span class="sxs-lookup"><span data-stu-id="0b3e8-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="0b3e8-110">I mapperuden i venstre side af Outlook-vinduet skal du vælge mappen Sendt post.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="0b3e8-111">Dobbeltklik på den meddelelse, du vil tilbagekalde, for at åbne den.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="0b3e8-112">Vælg fanen **meddelelse** , og vælg derefter **handlinger**  >  **Tilbagekald denne meddelelse**.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="0b3e8-113">Vælg **Slet ulæste kopier af denne meddelelse** , eller **Slet ulæste kopier, og Erstat med en ny meddelelse**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="0b3e8-114">Hvis du vil sende en erstatnings meddelelse, skal du skrive meddelelsen og derefter vælge **Send**.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="0b3e8-115">Det lykkedes eller ikke lykkedes at tilbagekalde en meddelelse, afhænger af modtagerens indstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="0b3e8-116">Du kan se, hvordan du kontrollerer tilbagekaldelsen, i [denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="0b3e8-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="0b3e8-117">Søg efter og slet mails i din organisation</span><span class="sxs-lookup"><span data-stu-id="0b3e8-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="0b3e8-118">Hvis du ikke er Global administrator, skal din konto føjes til rollen eDiscovery Manager-rolle eller overholdelses administrations rolle for at søge efter meddelelser.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="0b3e8-119">Hvis du vil slette meddelelser, skal du være medlem af gruppen organisations administrations rolle eller rollen søgning og sletning af administration.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="0b3e8-120">Tilladelser til disse roller tildeles i [sikkerheds-og overholdelses centeret](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="0b3e8-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="0b3e8-121">[Opret en indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/content-search) for at finde den besked, der skal slettes.</span><span class="sxs-lookup"><span data-stu-id="0b3e8-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="0b3e8-122">[Opret forbindelse til sikkerheds-og overholdelses Center-PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0b3e8-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="0b3e8-123">Hvis du bruger multifaktorgodkendelse, skal du se [oprette forbindelse til Microsoft 365 Security and Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0b3e8-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>