---
title: Offboard-enheder uden Windows fra Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744322"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="6968b-102">Offboard-enheder uden Windows fra Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="6968b-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="6968b-103">Sådan gør du:</span><span class="sxs-lookup"><span data-stu-id="6968b-103">Here's how:</span></span>

1. <span data-ttu-id="6968b-104">Følg tredjepartsdokumentationen for at afbryde tredjepartsløsningen fra Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="6968b-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="6968b-105">Fjern tilladelser for tredjepartsløsningen fra din Azure Active Directory-lejer:</span><span class="sxs-lookup"><span data-stu-id="6968b-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="6968b-106">Log på [Azure-portalen.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="6968b-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="6968b-107">Vælg **Alle tjenester i** Azure Active  >  **Directory**  >  **Enterprise-programmer.**</span><span class="sxs-lookup"><span data-stu-id="6968b-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="6968b-108">Vælg det program, du vil deaktivere.</span><span class="sxs-lookup"><span data-stu-id="6968b-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="6968b-109">Vælg **Slet.**</span><span class="sxs-lookup"><span data-stu-id="6968b-109">Select **Delete**.</span></span>

<span data-ttu-id="6968b-110">Hvis du vil have mere at vide, skal [du se Offboard-enheder uden for Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="6968b-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
