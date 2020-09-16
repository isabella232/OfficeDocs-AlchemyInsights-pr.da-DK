---
title: Finde mistede iOS-enheder med Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675150"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="84d72-102">Finde mistede iOS-enheder med Intune</span><span class="sxs-lookup"><span data-stu-id="84d72-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="84d72-103">Hvis du aktiverer tilstanden Hittegods på en iOS-enhed, kan en administrator have en meddelelse og et telefonnummer, der vises på låseskærmen.</span><span class="sxs-lookup"><span data-stu-id="84d72-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="84d72-104">Når tilstanden tabt er aktiveret, kan administratoren bruge handlingen Find enhed til at identificere enhedens fysiske placering.</span><span class="sxs-lookup"><span data-stu-id="84d72-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="84d72-105">Handlingen Find enhed i Intune fungerer med iOS-enheder for at vise placeringen af en bestemt enhed på et kort.</span><span class="sxs-lookup"><span data-stu-id="84d72-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="84d72-106">Hvis du bruger denne handling, skal iOS-enheden være i:</span><span class="sxs-lookup"><span data-stu-id="84d72-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="84d72-107">Overvåget tilstand</span><span class="sxs-lookup"><span data-stu-id="84d72-107">Supervised mode</span></span>
- <span data-ttu-id="84d72-108">Mistet tilstand</span><span class="sxs-lookup"><span data-stu-id="84d72-108">Lost mode</span></span>

<span data-ttu-id="84d72-109">Hvis du vil have mere at vide, skal du se [aktivere tilstanden tabt på iOS/iPadOS-enheder med Intune](https://docs.microsoft.com/intune/device-lost-mode) og [finde mistede eller stjålne iOS/iPadOS-enheder med Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="84d72-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="84d72-110">**Ofte stillede spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="84d72-110">**FAQ**</span></span>

<span data-ttu-id="84d72-111">Sp: Jeg har udsendt en fjernhandling for at fjerne firmadata fra en enhed, og nu sidder det fast i en afventende tilstand.</span><span class="sxs-lookup"><span data-stu-id="84d72-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="84d72-112">A: for at en fjernhandling kan fuldføres, skal den målrettede enhed være online og sunde.</span><span class="sxs-lookup"><span data-stu-id="84d72-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="84d72-113">I følgende situationer forbliver Fjernhandlingen i en afventende tilstand i 30 dage, eller indtil enheden godkender kommandoen:</span><span class="sxs-lookup"><span data-stu-id="84d72-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="84d72-114">Når enheden ikke har forbindelse</span><span class="sxs-lookup"><span data-stu-id="84d72-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="84d72-115">Når enheden mister sin administrations status med Intune</span><span class="sxs-lookup"><span data-stu-id="84d72-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="84d72-116">Hvis du tror, at en enhed ikke længere tjekkes ind, og at den ikke kan fjerne firmadata, skal du vælge Slet.</span><span class="sxs-lookup"><span data-stu-id="84d72-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="84d72-117">Sletning fjerner enhedsposten, så den ikke længere vises på listen over enheder i Intune.</span><span class="sxs-lookup"><span data-stu-id="84d72-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="84d72-118">Hvis enheden igen bliver aktiv, skal brugeren tilmelde den igen.</span><span class="sxs-lookup"><span data-stu-id="84d72-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="84d72-119">Sp: Hvorfor kan jeg ikke bruge visse fjernhandlinger?</span><span class="sxs-lookup"><span data-stu-id="84d72-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="84d72-120">En: ikke alle platforme understøtter alle handlinger med Fjern enheder.</span><span class="sxs-lookup"><span data-stu-id="84d72-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="84d72-121">Følgende fjernhandlinger er platformspecifikke, så de er kun tilgængelige for de platforme, der er angivet.</span><span class="sxs-lookup"><span data-stu-id="84d72-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="84d72-122">Tilsidesæt aktiverings låse (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="84d72-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="84d72-123">Ny start dato (kun Windows)</span><span class="sxs-lookup"><span data-stu-id="84d72-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="84d72-124">Tilstanden mistede (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="84d72-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="84d72-125">Find enhed (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="84d72-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="84d72-126">Genstart (kun Windows)</span><span class="sxs-lookup"><span data-stu-id="84d72-126">Restart (Windows only)</span></span>

<span data-ttu-id="84d72-127">Du kan finde flere oplysninger om hver handling under [tilgængelige enheds handlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="84d72-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>