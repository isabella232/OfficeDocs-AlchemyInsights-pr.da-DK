---
title: Oversigt over intune-enheder
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439158"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="6b672-102">Oversigt over intune-enheder</span><span class="sxs-lookup"><span data-stu-id="6b672-102">Intune Device Inventory</span></span>

<span data-ttu-id="6b672-103">Bladen Enheder giver administratoren indsigt i enheder under administration i Intune pr. enhed.</span><span class="sxs-lookup"><span data-stu-id="6b672-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="6b672-104">De viste oplysninger omfatter: Hardware, Fundne programmer, tilstand for overholdelse af enheden og tilstand for enhedskonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6b672-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="6b672-105">Lagerdata for hardware og fundne programmer indsamles på en syv-dages cyklus.</span><span class="sxs-lookup"><span data-stu-id="6b672-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="6b672-106">De programmer og specifikke elementer af hardware rapporteret varierer afhængigt af enhedens operativsystem, og om enheden er personligt eller corporate ejet.</span><span class="sxs-lookup"><span data-stu-id="6b672-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="6b672-107">Du kan finde flere oplysninger [under Oplysninger om enheden i Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="6b672-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="6b672-108">**Ofte stillede spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="6b672-108">**FAQ**</span></span>

<span data-ttu-id="6b672-109">Sp: Jeg modtager ikke en komplet oversigt over de programmer, der er til stede på Intune-tilmeldte Windows-enheder.</span><span class="sxs-lookup"><span data-stu-id="6b672-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="6b672-110">Hvorfor ikke?</span><span class="sxs-lookup"><span data-stu-id="6b672-110">Why not?</span></span>

<span data-ttu-id="6b672-111">A: På nuværende tidspunkt er det kun moderne apps, der er angivet til Windows 10-pc'er, der er identificeret som virksomhedsenheder.</span><span class="sxs-lookup"><span data-stu-id="6b672-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="6b672-112">Intune indsamler ikke oplysninger om Win32-apps, der er installeret på disse enheder.</span><span class="sxs-lookup"><span data-stu-id="6b672-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="6b672-113">Sp: Hvorfor indsamles telefonnumre ikke fra alle enheder?</span><span class="sxs-lookup"><span data-stu-id="6b672-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="6b672-114">A: Telefoner kategoriseret som virksomhedsenheder i Intune identificeres ikke med deres fulde telefonnummer, når du f.eks.</span><span class="sxs-lookup"><span data-stu-id="6b672-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="6b672-115">Bring-you-own-device telefonnumre er altid delvist maskeret med stjerner (\*\*\*\*), og viser kun de sidste fire cifre.</span><span class="sxs-lookup"><span data-stu-id="6b672-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>