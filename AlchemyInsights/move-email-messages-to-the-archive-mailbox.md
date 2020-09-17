---
title: Flyt mails til arkiv postkassen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799774"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="d7a5e-102">Flytte mails til arkiv postkassen</span><span class="sxs-lookup"><span data-stu-id="d7a5e-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="d7a5e-103">Hvis du vil have os til at køre automatiske tjek af de indstillinger, der er nævnt nedenfor, skal du vælge knappen tilbage <-øverst på denne side og derefter angive mailadressen på den bruger, der har problemer med at flytte mail til deres Arkiv postkasse.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="d7a5e-104">Bekræft, at en **Arkiv postkasse** er blevet aktiveret.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="d7a5e-105">Hvis ikke, skal du følge trinnene i [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) for at aktivere Arkiv postkassen.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="d7a5e-106">Hvis du vil arkivere meddelelser automatisk til arkiv postkassen, skal et opbevarings mærke med handlingen **Flyt til arkiv** være indstillet til **automatisk at blive anvendt på hele postkassen (standard)-mærket**.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="d7a5e-107">Følg trinnene her for at oprette mærket: [arkiverings standardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="d7a5e-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="d7a5e-108">Derefter skal du tilføje **Arkiv** mærket til opbevaringspolitikken.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="d7a5e-109">I Exchange Admin Center skal du vælge **opbevaringspolitikker** > føje **Flyt til arkiv-mærket** til politik > **gemme**.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="d7a5e-110">Nu kan du [tildele opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den pågældende brugers postkasse.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="d7a5e-111">Den samme politik anvendes på både den **primære** og den **arkiverede** postkasse.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="d7a5e-112">Det kan være nødvendigt at gennemtvinge, at MFA (Managed folder Assistant) kører og anvende de nye indstillinger i brugerens postkasse.</span><span class="sxs-lookup"><span data-stu-id="d7a5e-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="d7a5e-113">Kør følgende kommando, mens [du har forbindelse til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for at starte en administreret mappe assistent til en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="d7a5e-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="d7a5e-114">Start-ManagedFolderAssistant-id <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="d7a5e-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="d7a5e-115">Hvis du vil have mere at vide om konfiguration af en Arkiv politik, skal du se [konfigurere en arkiv-og sletnings politik for postkasser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="d7a5e-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  