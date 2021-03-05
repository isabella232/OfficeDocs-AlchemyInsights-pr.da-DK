---
title: Find hændelser, der udføres på indbakkeregler
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481716"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="ada5e-102">Find hændelser, der udføres på indbakkeregler</span><span class="sxs-lookup"><span data-stu-id="ada5e-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="ada5e-103">Når indbakkeregler oprettes, ændres eller slettes, registreres hændelserne i overvågningsloggen.</span><span class="sxs-lookup"><span data-stu-id="ada5e-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="ada5e-104">Sådan gennemgår du dem:</span><span class="sxs-lookup"><span data-stu-id="ada5e-104">Here's how to review them:</span></span>

1. <span data-ttu-id="ada5e-105">Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="ada5e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ada5e-106">Vælg Søg > søgning i overvågningsloggen.</span><span class="sxs-lookup"><span data-stu-id="ada5e-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ada5e-107">Hvis du ser en meddelelse om, at du skal aktivere overvågning, kan du aktivere det nu.</span><span class="sxs-lookup"><span data-stu-id="ada5e-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ada5e-108">Hvis denne funktion ikke er slået til, kan søgeresultaterne ikke trække data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="ada5e-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ada5e-109">Vælg feltet Aktiviteter, find Exchange-postkasseaktiviteter, og vælg derefter New-InboxRule Opret indbakkeregel fra Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="ada5e-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="ada5e-110">Når du er færdig, skal du klikke uden for ruden for at minimere ruden Aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="ada5e-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="ada5e-111">Angiv datointervallet, og vælg derefter brugernavnet for den bruger, du vil undersøge, i feltet Brugere.</span><span class="sxs-lookup"><span data-stu-id="ada5e-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="ada5e-112">Du kan vælge mere end én bruger ad gangen.</span><span class="sxs-lookup"><span data-stu-id="ada5e-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="ada5e-113">Vælg Søg.</span><span class="sxs-lookup"><span data-stu-id="ada5e-113">Select Search.</span></span> <span data-ttu-id="ada5e-114">Aktiviteterne vises under Resultater.</span><span class="sxs-lookup"><span data-stu-id="ada5e-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="ada5e-115">Hvis du vil have vist detaljer, skal du vælge en aktivitet og derefter vælge Flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="ada5e-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="ada5e-116">Under sektionen Parametre kan du se navnet på reglen, betingelser, der er angivet, og de handlinger, som reglen skal udføre.</span><span class="sxs-lookup"><span data-stu-id="ada5e-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="ada5e-117">Hvis du vil have mere at vide, skal du se Søge i Office 365-overvågningsloggen for at foretage fejlfinding af almindelige scenarier.</span><span class="sxs-lookup"><span data-stu-id="ada5e-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>