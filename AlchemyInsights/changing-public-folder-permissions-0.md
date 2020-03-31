---
title: Ændre tilladelser til offentlige mapper
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: 68aefd820c681a9022828f67655e1c843692a30e
ms.sourcegitcommit: 92e9a649532f5231ceedcafc4d14b8ad18d517c2
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/31/2020
ms.locfileid: "43059766"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="4be85-102">Ændre tilladelser til offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="4be85-102">Changing public folder permissions</span></span>

<span data-ttu-id="4be85-103">Tilladelser til offentlige mapper kan ændres af brugere og administratorer i Outlook.</span><span class="sxs-lookup"><span data-stu-id="4be85-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="4be85-104">Administratorer kan også styre tilladelser fra Exchange Administration (EAC) ved at gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="4be85-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="4be85-105">I Microsoft 365 Administration skal du gå til **Administration** \> **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4be85-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="4be85-106">Vælg **Offentlige mapper**.</span><span class="sxs-lookup"><span data-stu-id="4be85-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="4be85-107">Derfra kan du ændre tilladelser for individuelle offentlige mapper ved at tildele sikkerhedsgrupper til tilladelser.</span><span class="sxs-lookup"><span data-stu-id="4be85-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="4be85-108">Hvis en slutbruger skal ændre tilladelserne til offentlige mapper, skal brugeren have ejerrettigheder i mappen.</span><span class="sxs-lookup"><span data-stu-id="4be85-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="4be85-109">Følg den procedure, der er beskrevet i [Sådan diagnosticeres og løses tilladelser](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) til offentlige mapper for at foretage fejlfinding af problemer med tilladelser til offentlige mapper.</span><span class="sxs-lookup"><span data-stu-id="4be85-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="4be85-110">**Bemærk:** Der kan opstå flere kendte problemer, når du forsøger at ændre tilladelser for offentlige mapper.</span><span class="sxs-lookup"><span data-stu-id="4be85-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="4be85-111">Se følgende artikler for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="4be85-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="4be85-112">Tilladelser kan ikke anvendes på undermapper med offentlige mapper i EAC</span><span class="sxs-lookup"><span data-stu-id="4be85-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="4be85-113">Fejlen "Postkassen blev ikke fundet i det lokale område", når du får adgang til offentlige mapper</span><span class="sxs-lookup"><span data-stu-id="4be85-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
