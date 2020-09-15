---
title: 4c7-fejl i teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700197"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="072fb-102">4c7-fejl i Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="072fb-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="072fb-103">Denne fejl opstår, fordi Microsoft teams kræver formulargodkendelse.</span><span class="sxs-lookup"><span data-stu-id="072fb-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="072fb-104">Når du installerer Active Directory Federation Services (AD FS), er formulargodkendelse som standard ikke aktiveret for intranettet.</span><span class="sxs-lookup"><span data-stu-id="072fb-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="072fb-105">Hvis Windows-integreret godkendelse mislykkes, bliver du bedt om at logge på ved hjælp af formulargodkendelse.</span><span class="sxs-lookup"><span data-stu-id="072fb-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="072fb-106">For at løse dette problem skal du aktivere formulargodkendelse ved hjælp af MMC-snap-in'en AD FS (Microsoft Management Console) på den computer, der har den lokale kopi af Active Directory.</span><span class="sxs-lookup"><span data-stu-id="072fb-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="072fb-107">Dette gøres ved at benytte følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="072fb-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="072fb-108">I navigationsruden skal du gå til **godkendelsespolitikker**.</span><span class="sxs-lookup"><span data-stu-id="072fb-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="072fb-109">Under **handlinger** i ruden detaljer skal du vælge **Rediger global primær godkendelse**.</span><span class="sxs-lookup"><span data-stu-id="072fb-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="072fb-110">På fanen **intranet** skal du vælge **formulargodkendelse**.</span><span class="sxs-lookup"><span data-stu-id="072fb-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="072fb-111">Vælg **OK** (eller **Anvend**).</span><span class="sxs-lookup"><span data-stu-id="072fb-111">Select **OK** (or **Apply**).</span></span>