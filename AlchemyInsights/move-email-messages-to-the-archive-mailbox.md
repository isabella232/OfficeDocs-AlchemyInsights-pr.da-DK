---
title: Flytte mails til postkassen Arkiv
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522765"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="7336a-102">Flytte mail til arkivpostkassen</span><span class="sxs-lookup"><span data-stu-id="7336a-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="7336a-103">Hvis du vil have os til at køre automatiske kontroller for de indstillinger, der er nævnt nedenfor, skal du vælge tilbage-knappen < - øverst på denne side, og derefter indtaste e-mail-adressen på den bruger, der har problemer med at flytte e-mail til deres arkiv postkasse.</span><span class="sxs-lookup"><span data-stu-id="7336a-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="7336a-104">Bekræft, at **en arkivpostkasse** er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="7336a-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="7336a-105">Hvis ikke, skal du følge trinnene [i denne artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) for at aktivere arkivpostkassen.</span><span class="sxs-lookup"><span data-stu-id="7336a-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="7336a-106">Hvis du vil arkivere meddelelser automatisk i arkivpostkassen, skal en opbevaringskode **med handlingen Flyt** til arkiv indstilles til at **blive anvendt automatisk på hele postkassekoden (standardkode)**.</span><span class="sxs-lookup"><span data-stu-id="7336a-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="7336a-107">Brug trinnene her for at oprette tagget: [Arkivér standardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="7336a-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="7336a-108">Føj derefter **arkivkoden til** din opbevaringspolitik.</span><span class="sxs-lookup"><span data-stu-id="7336a-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="7336a-109">I Exchange Administration skal du vælge **Opbevaringspolitikker** > føje **tagget Flyt til arkiv** til politikken, > **gem**.</span><span class="sxs-lookup"><span data-stu-id="7336a-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="7336a-110">Tildel [nu opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse.</span><span class="sxs-lookup"><span data-stu-id="7336a-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="7336a-111">Den samme politik anvendes på både primær- **og** **arkivkassen** Arkiv.</span><span class="sxs-lookup"><span data-stu-id="7336a-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="7336a-112">Det kan være nødvendigt at tvinge MFA (Managed Folder Assistant) til at køre og anvende de nye indstillinger på brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="7336a-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="7336a-113">Kør følgende kommando, mens du [har oprettet forbindelse til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte assistenten For administreret mappe for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="7336a-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="7336a-114">Start-ManagedFolderAssistant -Identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="7336a-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="7336a-115">Du kan finde flere oplysninger om opsætning af en arkivpolitik [under Konfigurere en arkiv- og sletningspolitik for postkasser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="7336a-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  