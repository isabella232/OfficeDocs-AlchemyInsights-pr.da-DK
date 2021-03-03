---
title: Fjern data og aftørring af enheder fra Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416307"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="5ea17-102">Fjern data og aftørring af enheder fra Intune</span><span class="sxs-lookup"><span data-stu-id="5ea17-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="5ea17-103">Tilbagetrulning af enhed og fjernsletning af enhed kan bruges til at fjerne virksomhedsdata, der administreres af Intune, eller til at udføre en nulstilling til fabriksindstilling og returnere enheden til standardindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="5ea17-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="5ea17-104">Log på Microsoft 365 Enhedshåndtering, og gå til **Enheder**  >  **på alle enheder.**</span><span class="sxs-lookup"><span data-stu-id="5ea17-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="5ea17-105">Vælg den enhed, du vil slette.</span><span class="sxs-lookup"><span data-stu-id="5ea17-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="5ea17-106">Vælg den type fjernsletning, du vil udføre.</span><span class="sxs-lookup"><span data-stu-id="5ea17-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="5ea17-107">Tilbagetrækning sletter kun virksomhedsoplysninger, mens komplette sletninger gendanner enheden til fabriksindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="5ea17-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="5ea17-108">Vælg **Ja for** at bekræfte.</span><span class="sxs-lookup"><span data-stu-id="5ea17-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="5ea17-109">Indtil sletningen afsluttes, vises status for enhedshandlingen som Tilbagetrækning *afventer.*</span><span class="sxs-lookup"><span data-stu-id="5ea17-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="5ea17-110">Når handlingen er fuldført, kan du ikke længere se mobilenheden på listen over administrerede enheder.</span><span class="sxs-lookup"><span data-stu-id="5ea17-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="5ea17-111">Firmadata kan ikke fjernes fra enheder, DER ER FORBUNDET til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5ea17-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="5ea17-112">Du kan finde detaljerede oplysninger om effekten af handlingerne Tilbagetrækning og Sletning, herunder hvad der bevares, og hvad der slettes, i følgende dokumentation:</span><span class="sxs-lookup"><span data-stu-id="5ea17-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="5ea17-113">[Fjern enheder ved at slette, trække dem tilbage eller manuelt fjerne tilmeldingen af enheden.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)</span><span class="sxs-lookup"><span data-stu-id="5ea17-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="5ea17-114">Sådan slettes kun virksomhedsdata fra Intune-administrerede apps</span><span class="sxs-lookup"><span data-stu-id="5ea17-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="5ea17-115">[Slet alle data fra en macOS-enhed.](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)</span><span class="sxs-lookup"><span data-stu-id="5ea17-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>