---
title: Flytte mails til arkivpostkassen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822156"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="cdb46-102">Flytte mails til arkivpostkassen</span><span class="sxs-lookup"><span data-stu-id="cdb46-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="cdb46-103">Bekræft, at en **arkivpostkasse** er aktiveret.</span><span class="sxs-lookup"><span data-stu-id="cdb46-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="cdb46-104">Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til at aktivere arkivpostkassen.</span><span class="sxs-lookup"><span data-stu-id="cdb46-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="cdb46-105">Hvis du vil arkivere meddelelser automatisk i arkivpostkassen, skal en opbevaringskode med handlingen **Flyt til arkiv** være indstillet til **automatisk anvendt på hele postkasse koden (standard)**.</span><span class="sxs-lookup"><span data-stu-id="cdb46-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="cdb46-106">Brug trinnene her til at oprette tagget: [Arkiv standardtag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="cdb46-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="cdb46-107">Derefter skal du føje **arkiverings** tagget til din opbevaringspolitik.</span><span class="sxs-lookup"><span data-stu-id="cdb46-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="cdb46-108">I Exchange administration skal du vælge **opbevaringspolitikker** > føje **Flyt til arkiv-tagget** til politikken > **Gem**.</span><span class="sxs-lookup"><span data-stu-id="cdb46-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="cdb46-109">[Tildel nu opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den specifikke brugers postkasse.</span><span class="sxs-lookup"><span data-stu-id="cdb46-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="cdb46-110">Den samme politik vil blive anvendt på både den **primære** postkasse og **Arkiv** postkassen.</span><span class="sxs-lookup"><span data-stu-id="cdb46-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="cdb46-111">Det kan være nødvendigt at tvinge den administrerede mappe assistent (MFA) til at køre og anvende de nye indstillinger på brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="cdb46-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="cdb46-112">Kør følgende kommando, mens [du har forbindelse til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte den administrerede mappe assistent for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="cdb46-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="cdb46-113">Start-ManagedFolderAssistant-identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="cdb46-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="cdb46-114">Du finder flere oplysninger om, hvordan du konfigurerer en arkiveringspolitik, i [konfigurere en arkiverings-og sletningspolitik for postkasser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="cdb46-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  