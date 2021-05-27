---
title: Defender Endpoint kontrollerer sensorens status
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676099"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="f4ab1-102">Defender Endpoint kontrollerer sensorens status</span><span class="sxs-lookup"><span data-stu-id="f4ab1-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="f4ab1-103">Feltet **Enheder med sensorproblemer** findes på dashboardet Sikkerhedshandlinger.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="f4ab1-104">Dette felt indeholder oplysninger om den enkelte enheds mulighed for at levere sensordata og kommunikere med Defender for Endpoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="f4ab1-105">Den rapporterer, hvor mange enheder der kræver opmærksomhed, og hjælper dig med at identificere problematiske enheder og tage skridt til at rette kendte problemer.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="f4ab1-106">To statusindikatorer på feltet indeholder oplysninger om antallet af enheder, der ikke rapporterer korrekt til tjenesten:</span><span class="sxs-lookup"><span data-stu-id="f4ab1-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="f4ab1-107">**Forkert konfigureret** Enheder, der muligvis delvist rapporterer sensordata til Defender for Endpoint-tjenesten, og som muligvis har konfigurationsfejl, der skal rettes.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="f4ab1-108">**Inaktiv** Enheder, der er holdt op med at rapportere til Defender for Endpoint-tjenesten i mere end syv dage i den sidste måned.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="f4ab1-109">Når du klikker på en af grupperne, dirigeres du til listen Enheder, der er filtreret efter dine valg.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="f4ab1-110">På listen Enheder kan du filtrere listen over tilstandstilstande ud fra følgende status:</span><span class="sxs-lookup"><span data-stu-id="f4ab1-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="f4ab1-111">**Aktiv** Enheder, der aktivt rapporterer til Defender for Endpoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="f4ab1-112">**Forkert konfigureret** Enheder, der muligvis delvist rapporterer sensordata til Defender for Endpoint-tjenesten, men har konfigurationsfejl, der skal rettes.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="f4ab1-113">Forkert konfigurerede enheder kan have enten en eller en kombination af følgende problemer:</span><span class="sxs-lookup"><span data-stu-id="f4ab1-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="f4ab1-114">Ingen sensordata – Enheder er holdt op med at sende sensordata.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="f4ab1-115">Der kan udløses begrænsede beskeder fra enheden.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="f4ab1-116">Forringet kommunikation – Muligheden for at kommunikere med enheden er forringet.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="f4ab1-117">Det fungerer muligvis ikke at sende filer til dybdegående analyse, blokere filer, isolere enheden fra netværket og andre handlinger, der kræver kommunikation med enheden.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="f4ab1-118">**Inaktiv** Enheder, der er holdt op med at rapportere til Defender for Endpoint-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="f4ab1-119">Du kan downloade hele listen i CSV-format ved hjælp af funktionen Eksportér.</span><span class="sxs-lookup"><span data-stu-id="f4ab1-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="f4ab1-120">Du kan få mere at vide [under Kontrollér tilstanden for sensorens tilstand i Microsoft Defender til slutpunkt](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="f4ab1-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="f4ab1-121">Du kan finde flere oplysninger om, hvad der forårsagede, at en enhed var inaktiv eller forkert konfigureret, under Ret [usunde sensorer i Microsoft Defender til slutpunkt.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="f4ab1-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
