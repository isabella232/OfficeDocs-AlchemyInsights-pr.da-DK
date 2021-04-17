---
title: Fejl under oprettelse af livebegivenheder i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825509"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="b07fa-102">Fejl under oprettelse af livebegivenheder i Yammer</span><span class="sxs-lookup"><span data-stu-id="b07fa-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="b07fa-103">**Oprettelse af Yammer-livebegivenhed**</span><span class="sxs-lookup"><span data-stu-id="b07fa-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="b07fa-104">Yammer viser til enhver tid muligheden for at oprette en livebegivenhed.</span><span class="sxs-lookup"><span data-stu-id="b07fa-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="b07fa-105">I nogle tilfælde opfylder en bruger ikke forudsætningerne for at oprette en livebegivenhed og modtager en fejl, når der gøres forsøg på at oprette den.</span><span class="sxs-lookup"><span data-stu-id="b07fa-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="b07fa-106">Punkterne nedenfor dækker de almindelige årsager til dette problem og giver løsningsforslag til slutbrugere.</span><span class="sxs-lookup"><span data-stu-id="b07fa-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="b07fa-107">**Hvem kan oprette livebegivenheder**</span><span class="sxs-lookup"><span data-stu-id="b07fa-107">**Who can create live events**</span></span>
- <span data-ttu-id="b07fa-108">En Office 365 Enterprise E1-, E3- eller E5-licens eller en Office 365 A3- eller A5-licens.</span><span class="sxs-lookup"><span data-stu-id="b07fa-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="b07fa-109">Tilladelse til at oprette livebegivenheder i Microsoft Teams Administration.</span><span class="sxs-lookup"><span data-stu-id="b07fa-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="b07fa-110">Tilladelse til at oprette livebegivenheder i Microsoft Stream (for begivenheder, der er oprettet ved hjælp af en ekstern udsendelsesapp eller -enhed).</span><span class="sxs-lookup"><span data-stu-id="b07fa-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="b07fa-111">Fuldt teammedlemskab i organisationen (må ikke være gæst eller fra en anden organisation).</span><span class="sxs-lookup"><span data-stu-id="b07fa-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="b07fa-112">Privat mødeplanlægning, skærmdeling og IP-videodeling, slået til i Politik for teammøder.</span><span class="sxs-lookup"><span data-stu-id="b07fa-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="b07fa-113">**Politikker for oprettelse af livebegivenhed**</span><span class="sxs-lookup"><span data-stu-id="b07fa-113">**Live event creation policies**</span></span>

<span data-ttu-id="b07fa-114">Yammer følger de politikker for livebegivenheder, der er konfigureret i din Office 365-lejer til Stream.</span><span class="sxs-lookup"><span data-stu-id="b07fa-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="b07fa-115">Som standard kan alle i organisationen oprette en livebegivenhed.</span><span class="sxs-lookup"><span data-stu-id="b07fa-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="b07fa-116">Administratorer kan [ændre denne indstilling og dermed forhindre brugere i at oprette en livebegivenhed](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="b07fa-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="b07fa-117">Det er vigtigt at kontrollere, at brugerne har tilladelse til at oprette livebegivenheder, hvis de modtager en politikfejl.</span><span class="sxs-lookup"><span data-stu-id="b07fa-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
