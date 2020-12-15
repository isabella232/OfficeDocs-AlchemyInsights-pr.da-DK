---
title: 'Fejlfinding af voicemail '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677319"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="a4efc-102">Fejlfinding af voicemail</span><span class="sxs-lookup"><span data-stu-id="a4efc-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="a4efc-103">Sørg for, at funktionen optaget på optaget er bevidst.</span><span class="sxs-lookup"><span data-stu-id="a4efc-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="a4efc-104">Hvis denne funktion ikke er nødvendig for denne bruger:</span><span class="sxs-lookup"><span data-stu-id="a4efc-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="a4efc-105">Gå til [teams Administrationscenter](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="a4efc-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="a4efc-106">På den venstre bane skal du navigere i politikker for **tale**  >  **opkald**  >  **administrere politikker** for **Opkalds politikken**.</span><span class="sxs-lookup"><span data-stu-id="a4efc-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="a4efc-107">Vælg **Administrer brugere**.</span><span class="sxs-lookup"><span data-stu-id="a4efc-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="a4efc-108">Søg efter bruger, og ret opkalds politikken til en, der har **travlt optaget, er tilgængelig, når du ringer** til **fra**.</span><span class="sxs-lookup"><span data-stu-id="a4efc-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="a4efc-109">Klik på **Anvend**.</span><span class="sxs-lookup"><span data-stu-id="a4efc-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="a4efc-110">Ændringer af politikker kan tage op til 24 timer at replikere.</span><span class="sxs-lookup"><span data-stu-id="a4efc-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="a4efc-111">Hvis du vil have mere at vide om denne funktion, kan du se: [optaget på travl, når du er i gang med et opkald](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="a4efc-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
