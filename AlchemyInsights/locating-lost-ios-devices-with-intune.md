---
title: Lokalisering af mistede iOS-enheder med Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439142"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="e4e69-102">Lokalisering af mistede iOS-enheder med Intune</span><span class="sxs-lookup"><span data-stu-id="e4e69-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="e4e69-103">Aktivering af mistet tilstand på en iOS-enhed gør det muligt for en administrator at få vist en besked og et telefonnummer på låseskærmen.</span><span class="sxs-lookup"><span data-stu-id="e4e69-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="e4e69-104">Når tilstanden er gået tabt, kan administratoren bruge handlingen Find enhed til at identificere enhedens fysiske placering.</span><span class="sxs-lookup"><span data-stu-id="e4e69-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="e4e69-105">Handlingen Find enhed i Intune fungerer sammen med iOS-enheder for at vise placeringen af en bestemt enhed på et kort.</span><span class="sxs-lookup"><span data-stu-id="e4e69-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="e4e69-106">Brug af denne handling kræver, at iOS-enheden er i:</span><span class="sxs-lookup"><span data-stu-id="e4e69-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="e4e69-107">Overvåget tilstand</span><span class="sxs-lookup"><span data-stu-id="e4e69-107">Supervised mode</span></span>
- <span data-ttu-id="e4e69-108">Tilstanden Mistet</span><span class="sxs-lookup"><span data-stu-id="e4e69-108">Lost mode</span></span>

<span data-ttu-id="e4e69-109">Du kan finde flere oplysninger under [Aktivere mistet tilstand på iOS/iPadOS-enheder med Intune-](https://docs.microsoft.com/intune/device-lost-mode) og Find mistede eller stjålne [iOS/iPadOS-enheder med Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="e4e69-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="e4e69-110">**Ofte stillede spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="e4e69-110">**FAQ**</span></span>

<span data-ttu-id="e4e69-111">Sp: Jeg har udsendt en fjernhandling for at fjerne firmadata fra en enhed, og nu sidder den fast i en ventende tilstand.</span><span class="sxs-lookup"><span data-stu-id="e4e69-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="e4e69-112">A: For en ekstern handling for at fuldføre, den målrettede enhed skal være online og sund.</span><span class="sxs-lookup"><span data-stu-id="e4e69-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="e4e69-113">I følgende situationer forbliver fjernhandlingen i ventende tilstand i 30 dage, eller indtil enheden anerkender kommandoen:</span><span class="sxs-lookup"><span data-stu-id="e4e69-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="e4e69-114">Når enheden ikke har forbindelse</span><span class="sxs-lookup"><span data-stu-id="e4e69-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="e4e69-115">Når enheden mister sin administrationsstatus med Intune</span><span class="sxs-lookup"><span data-stu-id="e4e69-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="e4e69-116">Hvis du mener, at en enhed ikke længere tjekker ind, og at den ikke kan fjerne firmadata, skal du vælge Slet.</span><span class="sxs-lookup"><span data-stu-id="e4e69-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="e4e69-117">Hvis du sletter enheden, fjernes enhedsposten, så den ikke længere vises på listen Intune over enheder.</span><span class="sxs-lookup"><span data-stu-id="e4e69-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="e4e69-118">Hvis enheden bliver aktiv igen, skal brugeren tilmelde den igen.</span><span class="sxs-lookup"><span data-stu-id="e4e69-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="e4e69-119">Sp: Hvorfor er visse fjernhandlinger ikke tilgængelige for mig at bruge?</span><span class="sxs-lookup"><span data-stu-id="e4e69-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="e4e69-120">A: Ikke alle platforme understøtter alle eksterne enhedshandlinger.</span><span class="sxs-lookup"><span data-stu-id="e4e69-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="e4e69-121">Følgende fjernhandlinger er platformsspecifikke, så de er kun tilgængelige for de anbe bemærkede platforme.</span><span class="sxs-lookup"><span data-stu-id="e4e69-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="e4e69-122">Omgå aktiveringslås (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="e4e69-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="e4e69-123">Ny start (kun Windows)</span><span class="sxs-lookup"><span data-stu-id="e4e69-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="e4e69-124">Tilstanden Mistet (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="e4e69-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="e4e69-125">Find enhed (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="e4e69-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="e4e69-126">Genstart (kun Windows)</span><span class="sxs-lookup"><span data-stu-id="e4e69-126">Restart (Windows only)</span></span>

<span data-ttu-id="e4e69-127">Du kan finde flere oplysninger om hver handling under [Tilgængelige enhedshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="e4e69-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>