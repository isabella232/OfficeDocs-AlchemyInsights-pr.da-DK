---
title: Problemer med at fjerne en ikke-tavlet eller udkøret enhed fra Enhedens lager
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564169"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="68f59-102">Problemer med at fjerne en ikke-tavlet eller udkøret enhed fra Enhedens lager</span><span class="sxs-lookup"><span data-stu-id="68f59-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="68f59-103">Microsoft Defender til Slutpunkt tillader i øjeblikket ikke manuelt at fjerne enhedsposten for en offboardet eller ud afviklet enhed fra Lager over enheder.</span><span class="sxs-lookup"><span data-stu-id="68f59-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="68f59-104">Af sikkerhedsmæssige årsager forbliver enheden i portalen som en historisk post i op til 180 dage.</span><span class="sxs-lookup"><span data-stu-id="68f59-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="68f59-105">Men enhedens data slettes i henhold til din konfigurerede opbevaringsperiode.</span><span class="sxs-lookup"><span data-stu-id="68f59-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="68f59-106">**Bemærk!** En offboarded eller udkomponeret enhed skifter automatisk til **Inaktiv tilstand** efter syv dage.</span><span class="sxs-lookup"><span data-stu-id="68f59-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="68f59-107">Desuden tages enheder, der ikke er aktive inden for de seneste 30 dage, ikke med i de data, der afspejler din organisation Håndtering af trusler og sikkerhedsrisici eksponeringsscore eller Microsoft Secure Score for enheder.</span><span class="sxs-lookup"><span data-stu-id="68f59-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="68f59-108">Hvis du stadig ikke vil se visse enheder i visningen Lagerenhed, kan du prøve at placere et enhedsmærke for at filtrere den udkomne enhed fra visningen Lagerenhed.</span><span class="sxs-lookup"><span data-stu-id="68f59-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="68f59-109">Du kan finde flere oplysninger under:</span><span class="sxs-lookup"><span data-stu-id="68f59-109">For more information, see:</span></span>

[<span data-ttu-id="68f59-110">Offboard-enheder fra Microsoft Defender for Endpoint-tjenesten</span><span class="sxs-lookup"><span data-stu-id="68f59-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="68f59-111">Eksponeringsscore i Håndtering af trusler og sikkerhedsrisici</span><span class="sxs-lookup"><span data-stu-id="68f59-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="68f59-112">Ret usunde sensorerne i Microsoft Defender til Slutpunkt</span><span class="sxs-lookup"><span data-stu-id="68f59-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="68f59-113">Sådan bruges mærkning effektivt (del 1)</span><span class="sxs-lookup"><span data-stu-id="68f59-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="68f59-114">Sådan bruges mærkning effektivt (del 2)</span><span class="sxs-lookup"><span data-stu-id="68f59-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="68f59-115">Sådan bruges mærkning effektivt (del 3)</span><span class="sxs-lookup"><span data-stu-id="68f59-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




