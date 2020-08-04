---
title: Automatisk oprydning af forældede enheder i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554837"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="4a007-102">Automatisk oprydning af forældede enheder i Intune</span><span class="sxs-lookup"><span data-stu-id="4a007-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="4a007-103">Intune gør det muligt for administratoren at konfigurere et tidsinterval mellem 90 og 270 dage, hvorefter forældede enheder fjernes fra tjenesten.</span><span class="sxs-lookup"><span data-stu-id="4a007-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="4a007-104">Denne indstilling er hele organisationen, og når den er aktiveret, træder den i kraft med det samme.</span><span class="sxs-lookup"><span data-stu-id="4a007-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="4a007-105">Alle enheder, der ikke er tjekket ind på Intune-serveren i en periode, der overstiger indstillingen, slettes permanent.</span><span class="sxs-lookup"><span data-stu-id="4a007-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="4a007-106">**Bemærk:** Det er kun MDM-enhedsobjekter, der er berettiget til denne oprydningshandling.</span><span class="sxs-lookup"><span data-stu-id="4a007-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="4a007-107">Eas kun enhed objekter er udelukket.</span><span class="sxs-lookup"><span data-stu-id="4a007-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="4a007-108">Yderligere oplysninger om, hvornår en enhed bliver berettiget til sletning, er baseret på enhedens oprydningsindstilling og dens "tilstand":</span><span class="sxs-lookup"><span data-stu-id="4a007-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="4a007-109">Indstilling: **Slet enheder efter sidste indtjekningsdato: Ja (en vis værdi (N) i angivne dage)**</span><span class="sxs-lookup"><span data-stu-id="4a007-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="4a007-110">Baseret på værdi (N), der er konfigureret i indstillingen, sletter intune-tjenesten enheden i de angivne dage, efter at den sidst er blevet checket ind.</span><span class="sxs-lookup"><span data-stu-id="4a007-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="4a007-111">Indstilling: **Slet enheder efter sidste indtjekningsdato: Nej**</span><span class="sxs-lookup"><span data-stu-id="4a007-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="4a007-112">180 dage efter, at enhedscertifikatet udløber og ikke fornys, slettes enheden.</span><span class="sxs-lookup"><span data-stu-id="4a007-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="4a007-113">**Bemærk:** I begge tilfælde skal enheden være registreret i Intune.</span><span class="sxs-lookup"><span data-stu-id="4a007-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="4a007-114">Registrering sker under den første enheds checkin med Intune-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="4a007-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="4a007-115">Hvis en enhed tilmelder sig Intune, men ikke bliver Intune registreret, slettes enheden 270 dage efter tilmeldingen.</span><span class="sxs-lookup"><span data-stu-id="4a007-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="4a007-116">(90 dage til at markere enheden som tilbagekaldt og derefter yderligere 180 dage til at slette posten).</span><span class="sxs-lookup"><span data-stu-id="4a007-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="4a007-117">Der findes i øjeblikket ingen mekanisme i Intune-konsollen til at fastsætte udløbsdatoen for enhedscertificeringen for en given enhed.</span><span class="sxs-lookup"><span data-stu-id="4a007-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>