---
title: Flyt automatisk mails til arkivpostkassen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524098"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="25638-102">Flyt automatisk mails til arkivpostkassen</span><span class="sxs-lookup"><span data-stu-id="25638-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="25638-103">Sådan konfigurerer du en politik til automatisk at flytte en brugers gamle mail til arkivpostkassen:</span><span class="sxs-lookup"><span data-stu-id="25638-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="25638-104">Gå til [**Security & Arkiv for**](https://go.microsoft.com/fwlink/p/?linkid=2077143)overholdelse af  >    >  **datastyring for** at bekræfte, at en arkivpostkasse er aktiveret for brugeren.</span><span class="sxs-lookup"><span data-stu-id="25638-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="25638-105">Hvis den ikke er blevet vist, skal du **klikke på** **Aktivér og** derefter på Ja i advarselsfeltet.</span><span class="sxs-lookup"><span data-stu-id="25638-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="25638-106">Gå til [**Exchange Administration for > overholdelsesstyring > opbevaringsmærker.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="25638-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="25638-107">Vælg ikonet + og vælg derefter **automatisk anvend på hele postkassen.**</span><span class="sxs-lookup"><span data-stu-id="25638-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="25638-108">Tildel et navn til opbevaringsmærket, og vælg **Flyt til arkiv.**</span><span class="sxs-lookup"><span data-stu-id="25638-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="25638-109">For opbevaringsperioden skal du angive den ønskede tid, f.eks. 90 dage.</span><span class="sxs-lookup"><span data-stu-id="25638-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="25638-110">Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="25638-110">Click **Save**.</span></span>
5. <span data-ttu-id="25638-111">Opret nu en opbevaringspolitik: Vælg **opbevaringspolitikker,** vælg ikonet for at tilføje en ny politik.</span><span class="sxs-lookup"><span data-stu-id="25638-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="25638-112">Tildel et navn til opbevaringspolitikken, klik og rul derefter for at finde og tilføje det opbevaringsmærke, du lige har oprettet.</span><span class="sxs-lookup"><span data-stu-id="25638-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="25638-113">Klik på **Gem**.</span><span class="sxs-lookup"><span data-stu-id="25638-113">Click **Save**.</span></span>
7. <span data-ttu-id="25638-114">Til sidst skal du anvende opbevaringspolitikken på brugerens postkasse: Stadig i Exchange Administration skal du gå til **modtagernes**  >  **postkasser.**</span><span class="sxs-lookup"><span data-stu-id="25638-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="25638-115">Vælg alle de brugere, du vil anvende politikken på, og vælg derefter **Rediger** (blyantsikonet).</span><span class="sxs-lookup"><span data-stu-id="25638-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="25638-116">Klik på postkassefunktioner **i dialogboksen.**</span><span class="sxs-lookup"><span data-stu-id="25638-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="25638-117">Anvend **den politik,** du lige har oprettet, under Opbevaringspolitik > **Gem.**</span><span class="sxs-lookup"><span data-stu-id="25638-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="25638-118">Hvis du vil have vejledning i at anvende politikken på alle brugere, skal [du se Anvend en opbevaringspolitik på postkasser.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="25638-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
