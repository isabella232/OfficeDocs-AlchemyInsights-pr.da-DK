---
title: Kommentarer til listeelementer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982453"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="a60cf-102">Kommentarer til listeelementer</span><span class="sxs-lookup"><span data-stu-id="a60cf-102">Comments on List items</span></span>

<span data-ttu-id="a60cf-103">Brugerne vil snart kunne tilføje og slette kommentarer til listeelementer.</span><span class="sxs-lookup"><span data-stu-id="a60cf-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="a60cf-104">Brugere kan se alle kommentarer på et listeelement og filtrere mellem visninger, der viser kommentarer eller aktiviteter relateret til et element.</span><span class="sxs-lookup"><span data-stu-id="a60cf-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="a60cf-105">**Tidsindstilling** :</span><span class="sxs-lookup"><span data-stu-id="a60cf-105">**Timing** :</span></span>

<span data-ttu-id="a60cf-106">**Målrettet udgivelse** : gradvis rulning i midten af oktober og forventes at blive gennemført i midten-november</span><span class="sxs-lookup"><span data-stu-id="a60cf-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="a60cf-107">**Standard version** : gradvis rulning i midt-november og forventes at blive afsluttet i starten af december</span><span class="sxs-lookup"><span data-stu-id="a60cf-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="a60cf-108">**Udrulning** : målrettet udgivelse for hele organisationen</span><span class="sxs-lookup"><span data-stu-id="a60cf-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="a60cf-109">Brugerne skal bemærke følgende, før de kan tilføje og slette kommentarer:</span><span class="sxs-lookup"><span data-stu-id="a60cf-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="a60cf-110">Kommentarer følger de tilladelsesindstillinger, der er indbygget i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a60cf-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="a60cf-111">Klassiske lister, der endnu ikke er bygget til at blive vist i moderne brugergrænseflader, f. eks. opgavelister, vil ikke have denne kommentarfunktion.</span><span class="sxs-lookup"><span data-stu-id="a60cf-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="a60cf-112">Kommentering på lister i teams er ikke tilgængelig med denne version.</span><span class="sxs-lookup"><span data-stu-id="a60cf-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="a60cf-113">Kommentarer indekseres ikke ved søgning.</span><span class="sxs-lookup"><span data-stu-id="a60cf-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="a60cf-114">Administratorer kan deaktivere denne funktion på organisationsniveau ved at ændre **CommentsOnListItemsDisabled** -parameteren i cmdlet'en **set-SPOTenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a60cf-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="a60cf-115">Det er i øjeblikket ikke muligt at deaktivere kommentering på websteds-eller listeniveau.</span><span class="sxs-lookup"><span data-stu-id="a60cf-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="a60cf-116">Vi håber, at du har disse kontrolelementer i en senere opdatering, sandsynligt i den første kvartal 2021.</span><span class="sxs-lookup"><span data-stu-id="a60cf-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
