---
title: Find IP-adressen i overvågningsloggen
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481721"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="b463a-102">Find IP-adressen i overvågningsloggen</span><span class="sxs-lookup"><span data-stu-id="b463a-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="b463a-103">Den IP-adresse, der svarer til en aktivitet, der er udført af en bruger eller administrator, vises i overvågningsloggen.</span><span class="sxs-lookup"><span data-stu-id="b463a-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="b463a-104">Klientoplysningerne logføres også.</span><span class="sxs-lookup"><span data-stu-id="b463a-104">The client information is also logged.</span></span> <span data-ttu-id="b463a-105">Sådan identificerer du IP-adressen:</span><span class="sxs-lookup"><span data-stu-id="b463a-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="b463a-106">Gå til [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="b463a-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="b463a-107">Vælg **søgning i**  >  **[overvågningsloggen.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="b463a-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="b463a-108">Hvis du ser en meddelelse om, at du skal aktivere overvågning, kan du aktivere det nu.</span><span class="sxs-lookup"><span data-stu-id="b463a-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="b463a-109">Hvis denne funktion ikke er aktiveret, vil søgeresultaterne ikke kunne trække data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="b463a-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="b463a-110">Hvis du er interesseret i en bestemt aktivitet, skal du vælge den på **listen** Aktiviteter. Ellers returneres alle aktiviteter som standard for den valgte bruger.</span><span class="sxs-lookup"><span data-stu-id="b463a-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="b463a-111">Bemærk, at visse aktiviteter muligvis ikke kan vælges i **menuen** Aktiviteter. disse overvågningselementer returneres dog, hvis **Vis resultater for alle aktiviteter** er valgt (standardindstilling).</span><span class="sxs-lookup"><span data-stu-id="b463a-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="b463a-112">Angiv datointervallet, og vælg **brugernavnet for** den bruger, du vil undersøge, i feltet Brugere.</span><span class="sxs-lookup"><span data-stu-id="b463a-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="b463a-113">Vælg **Søg.**</span><span class="sxs-lookup"><span data-stu-id="b463a-113">Select **Search**.</span></span> <span data-ttu-id="b463a-114">Aktiviteterne vises under **Resultater.**</span><span class="sxs-lookup"><span data-stu-id="b463a-114">The activities appear under **Results**.</span></span> <span data-ttu-id="b463a-115">Du kan se IP-adressen for hver aktivitet.</span><span class="sxs-lookup"><span data-stu-id="b463a-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="b463a-116">Hvis du vil have vist detaljer, skal du vælge en aktivitet og derefter **vælge Flere oplysninger.**</span><span class="sxs-lookup"><span data-stu-id="b463a-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="b463a-117">Hvis du vil have mere at vide, skal du [se Søge i Office 365-overvågningsloggen for at foretage fejlfinding af almindelige scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="b463a-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>