---
title: Teams 4c7 fejl
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796040"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="c59ba-102">4c7-fejl i Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="c59ba-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="c59ba-103">Denne fejl opstår, fordi Microsoft teams kræver formulargodkendelse.</span><span class="sxs-lookup"><span data-stu-id="c59ba-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="c59ba-104">Når du implementerer Active Directory Federation Services (AD FS), er formulargodkendelse ikke aktiveret for intranettet som standard.</span><span class="sxs-lookup"><span data-stu-id="c59ba-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="c59ba-105">Hvis Windows-integreret godkendelse mislykkes, bliver du bedt om at logge på ved hjælp af formulargodkendelse.</span><span class="sxs-lookup"><span data-stu-id="c59ba-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="c59ba-106">Du kan lÃ ̧se problemet ved at aktivere formulargodkendelse ved hjÃ ¦ lp af snap-in'en AD FS Microsoft Management Console (MMC) pÃ ¥ den computer, der har den lokale kopi af Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c59ba-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="c59ba-107">Dette gøres ved at benytte følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="c59ba-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="c59ba-108">Gå til **godkendelsespolitikker**i navigationsruden.</span><span class="sxs-lookup"><span data-stu-id="c59ba-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="c59ba-109">Under **handlinger** i detaljeruden skal du vælge **Rediger global primær godkendelse**.</span><span class="sxs-lookup"><span data-stu-id="c59ba-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="c59ba-110">Vælg **formulargodkendelse**under fanen **intranet** .</span><span class="sxs-lookup"><span data-stu-id="c59ba-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="c59ba-111">Vælg **OK** (eller **Anvend**).</span><span class="sxs-lookup"><span data-stu-id="c59ba-111">Select **OK** (or **Apply**).</span></span>