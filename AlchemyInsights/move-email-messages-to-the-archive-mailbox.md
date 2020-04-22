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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713640"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="f2115-102">Flytte mail til arkivpostkassen</span><span class="sxs-lookup"><span data-stu-id="f2115-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="f2115-103">Bekræft, at en **arkivpostkasse** er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="f2115-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="f2115-104">Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til at aktivere arkivpostkassen.</span><span class="sxs-lookup"><span data-stu-id="f2115-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="f2115-105">Hvis du vil arkivere meddelelser automatisk til arkivpostkassen, skal et opbevaringsmærke med handlingen **Flyt til arkiv** angives til **automatisk at blive anvendt på hele postkassekoden (standard).**</span><span class="sxs-lookup"><span data-stu-id="f2115-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="f2115-106">Følg trinnene her for at oprette mærket: [Arkivstandardkode](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="f2115-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="f2115-107">Derefter skal du føje **arkivtagget** til din opbevaringspolitik.</span><span class="sxs-lookup"><span data-stu-id="f2115-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="f2115-108">I Exchange Administration skal du vælge **Opbevaringspolitikker >** føje **tagget Flyt til arkiv** til politikken > **Gem**.</span><span class="sxs-lookup"><span data-stu-id="f2115-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="f2115-109">[Tildel nu opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse.</span><span class="sxs-lookup"><span data-stu-id="f2115-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="f2115-110">Den samme politik anvendes på både postkassen **Primær** og **Arkiv.**</span><span class="sxs-lookup"><span data-stu-id="f2115-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="f2115-111">Det kan være nødvendigt at tvinge MFA (Managed Folder Assistant) til at køre og anvende de nye indstillinger på brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="f2115-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="f2115-112">Kør følgende kommando, mens [du har forbindelse til EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte Assistent til administrerede mapper for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="f2115-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="f2115-113">Start-ManagedFolderAssistant -Identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="f2115-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="f2115-114">Du kan finde flere oplysninger om opsætning af en arkivpolitik [under Konfigurere en arkiv- og sletningspolitik for postkasser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="f2115-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  