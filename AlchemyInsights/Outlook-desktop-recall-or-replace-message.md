---
title: Tilbagekaldelse eller erstatning af en mail til Outlook-skrivebordet
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687504"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="127c7-102">Tilbagekalde eller erstatte en Outlook-mail</span><span class="sxs-lookup"><span data-stu-id="127c7-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="127c7-103">Som administrator kan du **tilbagekalde meddelelser på vegne af brugere, der bruger PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="127c7-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="127c7-104">Du kan ikke tilbagekalde meddelelser fra Administration.</span><span class="sxs-lookup"><span data-stu-id="127c7-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="127c7-105">Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**.</span><span class="sxs-lookup"><span data-stu-id="127c7-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="127c7-106">Hvis meddelelsen blev sendt til en Gmail-adresse, kan du f.eks.</span><span class="sxs-lookup"><span data-stu-id="127c7-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="127c7-107">Du kan **kun tilbagekalde meddelelser, der er sendt fra Outlook 2016 på pc'en**.</span><span class="sxs-lookup"><span data-stu-id="127c7-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="127c7-108">Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke huske den.</span><span class="sxs-lookup"><span data-stu-id="127c7-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="127c7-109">Sådan tilbagekaldes eller erstattes en mail:</span><span class="sxs-lookup"><span data-stu-id="127c7-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="127c7-110">Vælg mappen Sendt post i mapperuden til venstre i Outlook-vinduet.</span><span class="sxs-lookup"><span data-stu-id="127c7-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="127c7-111">Dobbeltklik på den meddelelse, du vil tilbagekalde, for at åbne den.</span><span class="sxs-lookup"><span data-stu-id="127c7-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="127c7-112">Vælg fanen **Meddelelse,** og vælg derefter **Handlinger** > **Genkald denne meddelelse**.</span><span class="sxs-lookup"><span data-stu-id="127c7-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="127c7-113">Vælg **Slet ulæste kopier af denne meddelelse** eller Slet **ulæste kopier, og erstat med en ny meddelelse**, og vælg derefter **OK**.</span><span class="sxs-lookup"><span data-stu-id="127c7-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="127c7-114">Hvis du sender en erstatningsmeddelelse, skal du skrive meddelelsen og derefter vælge **Send**.</span><span class="sxs-lookup"><span data-stu-id="127c7-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="127c7-115">En tilbagekaldelse af en meddelelses succes eller fiasko afhænger af modtagerens indstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="127c7-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="127c7-116">Du kan se, hvordan du kontrollerer tilbagekaldelsen, i [denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="127c7-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="127c7-117">Søge efter og slette mails i din organisation</span><span class="sxs-lookup"><span data-stu-id="127c7-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="127c7-118">Hvis du ikke er global administrator, skal din konto føjes til rollen eDiscovery Manager eller rollen Styring af overholdelsessøgning for at søge efter meddelelser.</span><span class="sxs-lookup"><span data-stu-id="127c7-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="127c7-119">Hvis du vil slette meddelelser, skal du deltage i rollegruppen Organisationsstyring eller rollen Administration af søgning og sletning.</span><span class="sxs-lookup"><span data-stu-id="127c7-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="127c7-120">Tilladelser til disse roller tildeles i [Sikkerheds- og overholdelsescenter](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="127c7-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="127c7-121">[Opret en indholdssøgning](https://docs.microsoft.com/office365/securitycompliance/content-search) for at finde den meddelelse, der skal slettes.</span><span class="sxs-lookup"><span data-stu-id="127c7-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="127c7-122">[Opret forbindelse til PowerShell til Sikkerheds- og Compliance Center](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="127c7-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="127c7-123">Hvis du bruger multifaktorgodkendelse, skal du se [Oprette forbindelse til Microsoft 365-sikkerhed og Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="127c7-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>