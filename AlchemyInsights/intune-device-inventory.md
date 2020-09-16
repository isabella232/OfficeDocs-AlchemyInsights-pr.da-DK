---
title: Oversigt over Intune-enheder
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667872"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="c6896-102">Oversigt over Intune-enheder</span><span class="sxs-lookup"><span data-stu-id="c6896-102">Intune Device Inventory</span></span>

<span data-ttu-id="c6896-103">Device-bladet giver administrator indsigt i enheder under administration i Intune på et enkelt enheds grundlag.</span><span class="sxs-lookup"><span data-stu-id="c6896-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="c6896-104">De oplysninger, der vises, omfatter: hardware, registrerede programmer, enheds kompatibilitetstilstand og enheds konfigurationstilstand.</span><span class="sxs-lookup"><span data-stu-id="c6896-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="c6896-105">Lagerdata for hardware og opdagede programmer indsamles på en 7-dages cyklus.</span><span class="sxs-lookup"><span data-stu-id="c6896-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="c6896-106">Programmer og specifikke elementer af hardware, der rapporteres, varierer afhængigt af enhedens operativsystem, og om enheden er personligt eller firma ejet.</span><span class="sxs-lookup"><span data-stu-id="c6896-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="c6896-107">Hvis du vil have mere at vide, skal du se [få vist enhedsoplysninger i Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="c6896-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="c6896-108">**Ofte stillede spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="c6896-108">**FAQ**</span></span>

<span data-ttu-id="c6896-109">Sp: Jeg modtager ikke en komplet oversigt over programmer, der er tilgængelige på de Intune-registrerede Windows-enheder.</span><span class="sxs-lookup"><span data-stu-id="c6896-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="c6896-110">Hvorfor ikke?</span><span class="sxs-lookup"><span data-stu-id="c6896-110">Why not?</span></span>

<span data-ttu-id="c6896-111">A: på nuværende tidspunkt vises kun moderne apps til Windows 10-pc'er, der er identificeret som virksomhedens enheder.</span><span class="sxs-lookup"><span data-stu-id="c6896-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="c6896-112">Intune indsamler ikke oplysninger om de Win32-apps, der er installeret på disse enheder.</span><span class="sxs-lookup"><span data-stu-id="c6896-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="c6896-113">Sp: Hvorfor indsamles der ikke telefonnumre fra alle enheder?</span><span class="sxs-lookup"><span data-stu-id="c6896-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="c6896-114">En: telefoner, der er kategoriseret som virksomhedsenheder i Intune, identificeres ikke med deres fulde telefonnummer, når du for eksempel kører en lager rapport fra en mobil enhed.</span><span class="sxs-lookup"><span data-stu-id="c6896-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="c6896-115">Sæt telefonnumre til telefonenheder er altid delvist afmasket med asterisk (\* \* \* \*), og kun de sidste fire cifre vises.</span><span class="sxs-lookup"><span data-stu-id="c6896-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>