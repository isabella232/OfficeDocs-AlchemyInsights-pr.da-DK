---
title: Fjerne data og slette enheder fra Intune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701277"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="3ffdd-102">Fjerne data og slette enheder fra Intune</span><span class="sxs-lookup"><span data-stu-id="3ffdd-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="3ffdd-103">Aflevering af enheden og fjernhandlinger til sletning af enheder kan bruges til at fjerne virksomhedsdata, der administreres af Intune, eller til at udføre en Fabriks nulstilling og sætte enheden tilbage til standardindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="3ffdd-104">Log på Microsoft 365-Enhedsadministration, og gå til **enheder**på  >  **alle enheder**.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="3ffdd-105">Vælg den enhed, du vil slette.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="3ffdd-106">Vælg den type Fjern sletning, du vil udføre.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="3ffdd-107">Tilbagetrækning sletter kun organisationsoplysninger, mens alle sletninger gendanner enheden til fabriksindstillingerne.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="3ffdd-108">Vælg **Ja** for at bekræfte.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="3ffdd-109">Indtil sletningen er fuldført, vises status for enheds handlingen som afventer tilbagetrækning.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="3ffdd-110">Når handlingen er fuldført, kan du ikke længere se mobilenheden på listen over administrerede enheder.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="3ffdd-111">**Bemærk!** Firmadata kan ikke fjernes fra enheder, der er knyttet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3ffdd-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="3ffdd-112">Hvis du vil have detaljerede oplysninger om effekten af aftræks-og slette handlingerne, herunder hvad der bevares, og hvad der slettes, skal du se [fjerne enheder ved hjælp af slet, Fjern eller Fjern registreringen af enheden manuelt](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="3ffdd-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="3ffdd-113">Hvis du vil slette alle data fra en macOS-enhed, skal du se [Slet alle data fra en macOS-enhed](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="3ffdd-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>