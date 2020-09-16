---
title: Automatisk oprydning af gamle enheder i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715015"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="803ed-102">Automatisk oprydning af gamle enheder i Intune</span><span class="sxs-lookup"><span data-stu-id="803ed-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="803ed-103">Intune gør det muligt for administratoren at konfigurere et tidsinterval mellem 90 og 270 dage, hvorefter der fjernes fejl enheder fra tjenesten.</span><span class="sxs-lookup"><span data-stu-id="803ed-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="803ed-104">Denne indstilling er organisations bredden, og når aktiveret træder i kraft med det samme.</span><span class="sxs-lookup"><span data-stu-id="803ed-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="803ed-105">Enheder, der ikke er markeret i Intune-serveren for en periode, der overskrider indstillingen, slettes permanent.</span><span class="sxs-lookup"><span data-stu-id="803ed-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="803ed-106">**Bemærk!** Kun MDM-enhedsobjekter er berettiget til denne oprydnings handling.</span><span class="sxs-lookup"><span data-stu-id="803ed-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="803ed-107">Kun EA Device Objects er udeladt.</span><span class="sxs-lookup"><span data-stu-id="803ed-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="803ed-108">Du kan finde flere oplysninger om, hvornår en enhed bliver kvalificeret til at blive slettet baseret på indstillingen for oprydning af enheder og dens "tilstand":</span><span class="sxs-lookup"><span data-stu-id="803ed-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="803ed-109">Indstilling: **Slet enheder efter sidste checkdato: Ja (nogle af værdierne (N) i dage angivet)**</span><span class="sxs-lookup"><span data-stu-id="803ed-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="803ed-110">Baseret på værdi (N), der er konfigureret i indstillingen, sletter tjenesten Intune enheden i de dage, efter den sidst blev gennemført.</span><span class="sxs-lookup"><span data-stu-id="803ed-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="803ed-111">Indstilling:  **Slet enheder efter sidste indtjekning-dato: Nej**</span><span class="sxs-lookup"><span data-stu-id="803ed-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="803ed-112">180 dage efter at enheds certifikatet udløber og ikke fornys, slettes enheden.</span><span class="sxs-lookup"><span data-stu-id="803ed-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="803ed-113">**Bemærk!** I begge tilfælde skal enheden registreres korrekt i Intune.</span><span class="sxs-lookup"><span data-stu-id="803ed-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="803ed-114">Registrering sker under første enheds indtjekning med Intune-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="803ed-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="803ed-115">Hvis en enhed er tilmeldt Intune, men ikke bliver registreret som Intune, slettes enheden 270 dage efter tilmeldingen.</span><span class="sxs-lookup"><span data-stu-id="803ed-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="803ed-116">(90 dage for at markere enheden som tilbagekaldt og derefter en anden 180 dage for at slette posten.)</span><span class="sxs-lookup"><span data-stu-id="803ed-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="803ed-117">Der findes i øjeblikket ingen mekanisme i Intune-konsollen til at oprette udløbsdatoen for enheds certificeringen for en given enhed.</span><span class="sxs-lookup"><span data-stu-id="803ed-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>