---
title: Bloker bruger fra at optage møder
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035368"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="ce78a-102">Bloker bruger fra at optage møder</span><span class="sxs-lookup"><span data-stu-id="ce78a-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="ce78a-103">Hvis du har brug for **at forhindre eller blokere** bestemte brugere i at optage Teams-møder, kan du gøre det via politikindstillinger for Teams-møder.</span><span class="sxs-lookup"><span data-stu-id="ce78a-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="ce78a-104">I Microsoft Teams Administration skal du deaktivere indstillingen Tillad optagelse i **skyen i** den mødepolitik, der er tildelt den pågældende bruger.</span><span class="sxs-lookup"><span data-stu-id="ce78a-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="ce78a-105">Hvis du vil have mere at vide, [skal du se Administrer mødepolitikker i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="ce78a-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="ce78a-106">Hvis du vil validere, om en bestemt bruger har tilladelse til eller ikke at optage Teams-møder, skal du bruge supportdiagnosticering.</span><span class="sxs-lookup"><span data-stu-id="ce78a-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="ce78a-107">Kør en ny supportforespørgsel, og skriv **Diag:** Mødeoptagelse – diagnosticeringsværktøjet kontrollerer politikindstillingerne for den angivne bruger og bestemmer deres politikindstillinger.</span><span class="sxs-lookup"><span data-stu-id="ce78a-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="ce78a-108">Husk, at det kan tage et par timer, før nye politikindstillinger træder i kraft, så hvis du lige har foretaget en ændring, skal du vente et par timer, før du kører diagnosticeringen igen.</span><span class="sxs-lookup"><span data-stu-id="ce78a-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="ce78a-109">Hvis du vil have mere at vide, [skal du gennemse Slå skyoptagelse til eller fra.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="ce78a-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
