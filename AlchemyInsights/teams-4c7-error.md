---
title: Teams 4c7-fejl
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786663"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="6dfdc-102">4c7-fejl i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6dfdc-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="6dfdc-103">Denne fejl opstår, fordi Microsoft Teams kræver Formulargodkendelse.</span><span class="sxs-lookup"><span data-stu-id="6dfdc-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="6dfdc-104">Når du installerer Active Directory Federation Services (AD FS), er formulargodkendelse ikke aktiveret på intranettet som standard.</span><span class="sxs-lookup"><span data-stu-id="6dfdc-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="6dfdc-105">Hvis Windows-integreret godkendelse mislykkes, bliver du bedt om at logge på ved hjælp af formulargodkendelse.</span><span class="sxs-lookup"><span data-stu-id="6dfdc-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="6dfdc-106">Du kan løse dette problem ved at aktivere formulargodkendelse ved hjælp af AD FS Microsoft Management Console-snap-in'en (MMC) på den computer, der har den lokale kopi af Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6dfdc-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="6dfdc-107">Dette gøres ved at benytte følgende fremgangsmåde:</span><span class="sxs-lookup"><span data-stu-id="6dfdc-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="6dfdc-108">I navigationsruden skal du gå til **Godkendelsespolitikker**.</span><span class="sxs-lookup"><span data-stu-id="6dfdc-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="6dfdc-109">Under **Handlinger** i detaljeruden skal du vælge **Rediger global primær godkendelse.**</span><span class="sxs-lookup"><span data-stu-id="6dfdc-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="6dfdc-110">På fanen **Intranet** skal du vælge **Formulargodkendelse**.</span><span class="sxs-lookup"><span data-stu-id="6dfdc-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="6dfdc-111">Vælg **OK** (eller **Anvend).**</span><span class="sxs-lookup"><span data-stu-id="6dfdc-111">Select **OK** (or **Apply**).</span></span>