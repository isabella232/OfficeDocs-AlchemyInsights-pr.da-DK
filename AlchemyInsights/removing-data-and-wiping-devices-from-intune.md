---
title: Fjernelse af data og aftørring af enheder fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439157"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="990df-102">Fjernelse af data og aftørring af enheder fra Intune</span><span class="sxs-lookup"><span data-stu-id="990df-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="990df-103">Fjernhandlingerne Device Retire og Device Wipe kan bruges til at fjerne firmadata, der administreres af Intune, eller til at udføre en fabriksnulstilling og returnere enheden til standardindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="990df-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="990df-104">Log på Microsoft 365 Device Management, og gå til **Enheder**  >  **alle enheder**.</span><span class="sxs-lookup"><span data-stu-id="990df-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="990df-105">Vælg den enhed, du vil slette.</span><span class="sxs-lookup"><span data-stu-id="990df-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="990df-106">Vælg den type fjernsletning, du vil udføre.</span><span class="sxs-lookup"><span data-stu-id="990df-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="990df-107">Udgå sletter kun organisatoriske oplysninger, mens fuld klude gendanne enheden til sine fabriksindstillinger.</span><span class="sxs-lookup"><span data-stu-id="990df-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="990df-108">Vælg **Ja for** at bekræfte.</span><span class="sxs-lookup"><span data-stu-id="990df-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="990df-109">Indtil sletningen er færdig, vises statussen Enhedshandling som Afventer pension.</span><span class="sxs-lookup"><span data-stu-id="990df-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="990df-110">Når handlingen er fuldført, kan du ikke længere se mobilenheden på listen over administrerede enheder.</span><span class="sxs-lookup"><span data-stu-id="990df-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="990df-111">**Bemærk:** Virksomhedsdata kan ikke fjernes fra enheder, der er tilsluttet Azure AD.</span><span class="sxs-lookup"><span data-stu-id="990df-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="990df-112">Du kan finde alle oplysninger om effekten af handlingerne Gå på pension og slette, herunder hvad der bevares, og hvad der slettes, under Fjerne enheder [ved hjælp af sletning, udgå eller automatisk](https://docs.microsoft.com/intune/devices-wipe)fjernelse af enheden .</span><span class="sxs-lookup"><span data-stu-id="990df-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="990df-113">Hvis du vil slette alle data fra en macOS-enhed, skal [du se Slette alle data fra en macOS-enhed](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="990df-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>