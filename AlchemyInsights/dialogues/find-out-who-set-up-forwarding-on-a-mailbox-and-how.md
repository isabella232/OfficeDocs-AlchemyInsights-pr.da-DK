---
title: Find ud af, hvem der har konfigureret videresendelse på en postkasse, og hvordan
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429418"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="acd6a-102">Find ud af, hvem der har konfigureret videresendelse på en postkasse, og hvordan</span><span class="sxs-lookup"><span data-stu-id="acd6a-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="acd6a-103">Hvis ekstern videresendelse blev angivet på en postkasse, overvåges aktiviteten som en del Set-Mailbox cmdlet'en.</span><span class="sxs-lookup"><span data-stu-id="acd6a-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="acd6a-104">Sådan finder du aktiviteten i overvågningsloggen:</span><span class="sxs-lookup"><span data-stu-id="acd6a-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="acd6a-105">Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="acd6a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="acd6a-106">Vælg **søgning i** >  **overvågningsloggen.**</span><span class="sxs-lookup"><span data-stu-id="acd6a-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="acd6a-107">Hvis du ser en meddelelse om, at du skal aktivere overvågning, kan du aktivere det nu.</span><span class="sxs-lookup"><span data-stu-id="acd6a-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="acd6a-108">Hvis denne funktion ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="acd6a-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="acd6a-109">Sørg for, **at feltet** Aktiviteter er indstillet **til At vise resultater for alle aktiviteter** (standarden).</span><span class="sxs-lookup"><span data-stu-id="acd6a-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="acd6a-110">Angiv datointervallet.</span><span class="sxs-lookup"><span data-stu-id="acd6a-110">Specify the date range.</span></span> <span data-ttu-id="acd6a-111">Du behøver ikke at angive et brugernavn.</span><span class="sxs-lookup"><span data-stu-id="acd6a-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="acd6a-112">Vælg **Søg.**</span><span class="sxs-lookup"><span data-stu-id="acd6a-112">Select **Search**.</span></span> <span data-ttu-id="acd6a-113">Aktiviteterne vises under **Resultater.**</span><span class="sxs-lookup"><span data-stu-id="acd6a-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="acd6a-114">Vælg **Filtrer** resultater, og angiv **derefter Set-mailbox** i **feltet Aktivitetsfilter.**</span><span class="sxs-lookup"><span data-stu-id="acd6a-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="acd6a-115">Dette returnerer alle **Set-Mailbox-aktiviteter.**</span><span class="sxs-lookup"><span data-stu-id="acd6a-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="acd6a-116">Hvis du vil have vist detaljerne, skal du vælge en aktivitet og derefter **vælge Flere oplysninger.**</span><span class="sxs-lookup"><span data-stu-id="acd6a-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="acd6a-117">Under **Parametre** kan du se den mailadresse til videresendelse, der blev angivet på postkassen.</span><span class="sxs-lookup"><span data-stu-id="acd6a-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="acd6a-118">**Bruger-id'et** repræsenterer den bruger, der har konfigureret ekstern videresendelse på postkassen.</span><span class="sxs-lookup"><span data-stu-id="acd6a-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="acd6a-119">Hvis du vil have mere at vide, [skal du se Søge i Office 365-overvågningsloggen for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="acd6a-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>