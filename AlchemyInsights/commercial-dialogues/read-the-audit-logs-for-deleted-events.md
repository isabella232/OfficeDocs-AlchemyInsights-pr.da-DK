---
title: Læs overvågningslogfilerne for slettede hændelser
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481556"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="b85be-102">Læs overvågningslogfilerne for slettede hændelser</span><span class="sxs-lookup"><span data-stu-id="b85be-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="b85be-103">Sådan gør du:</span><span class="sxs-lookup"><span data-stu-id="b85be-103">Here's how to do this:</span></span>

1. <span data-ttu-id="b85be-104">Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="b85be-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="b85be-105">Vælg **søgning i**  >  [**overvågningsloggen.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="b85be-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="b85be-106">Hvis du ser en meddelelse om, at du skal aktivere funktionen, kan du aktivere den nu.</span><span class="sxs-lookup"><span data-stu-id="b85be-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="b85be-107">Hvis funktionen ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="b85be-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="b85be-108">Vælg **Aktiviteter,** og find derefter Aktiviteter i **Exchange-postkassen.**</span><span class="sxs-lookup"><span data-stu-id="b85be-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="b85be-109">Markér **slettede meddelelser fra mappen Slettet post** og Flyttede meddelelser til indstillingerne for **mappen** Slettet post.</span><span class="sxs-lookup"><span data-stu-id="b85be-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="b85be-110">Når du er færdig, skal du klikke uden for ruden for at minimere **ruden** Aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="b85be-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="b85be-111">Angiv datointervallet, og vælg derefter **brugernavnet** for den bruger, du vil undersøge, i feltet Brugere.</span><span class="sxs-lookup"><span data-stu-id="b85be-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="b85be-112">Du kan vælge mere end én bruger ad gangen.</span><span class="sxs-lookup"><span data-stu-id="b85be-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="b85be-113">Vælg **Søg.**</span><span class="sxs-lookup"><span data-stu-id="b85be-113">Select **Search**.</span></span> <span data-ttu-id="b85be-114">Aktiviteterne vises under **Resultater.**</span><span class="sxs-lookup"><span data-stu-id="b85be-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="b85be-115">Hvis du vil have vist detaljerne, skal du vælge en aktivitet og derefter **vælge Flere oplysninger.**</span><span class="sxs-lookup"><span data-stu-id="b85be-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="b85be-116">Yderligere oplysninger om det slettede element, f.eks. emnelinjen og placeringen af elementet,  da det blev slettet, vises i feltet PåvirkedeWebsteder.</span><span class="sxs-lookup"><span data-stu-id="b85be-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="b85be-117">Du kan ikke gendanne slettede elementer ved hjælp af overvågningslogfunktionen.</span><span class="sxs-lookup"><span data-stu-id="b85be-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="b85be-118">Hvis du vil gendanne slettede elementer, skal [du se Gendan slettede elementer eller mail i Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="b85be-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="b85be-119">Hvis du vil have mere at vide, [skal du se Søge i Office 365-overvågningsloggen for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="b85be-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
