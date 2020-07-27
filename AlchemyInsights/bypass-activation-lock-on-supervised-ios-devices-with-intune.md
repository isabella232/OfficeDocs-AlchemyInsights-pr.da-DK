---
title: Omgå aktiveringslås på overvågede iOS-enheder med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423491"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="8c13f-102">Omgå aktiveringslås på overvågede iOS-enheder med Intune</span><span class="sxs-lookup"><span data-stu-id="8c13f-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="8c13f-103">Muligheden for at omgå aktiveringslåsen på iOS-enheder gør det nemmere at komme sig efter det scenario, hvor en bruger aktiverer aktiveringslås på en virksomhedsenhed, og forlader derefter virksomheden.</span><span class="sxs-lookup"><span data-stu-id="8c13f-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="8c13f-104">Forudsætninger for at omgå en aktiveringslås omfatter:</span><span class="sxs-lookup"><span data-stu-id="8c13f-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="8c13f-105">En enhed er, der er "overvåget".</span><span class="sxs-lookup"><span data-stu-id="8c13f-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="8c13f-106">Aktiveringslåsen er aktiveret ved hjælp af begrænsningspolitikken for iOS-enheder i Intune.</span><span class="sxs-lookup"><span data-stu-id="8c13f-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="8c13f-107">Når du omgår en aktiveringslås, skal du desuden:</span><span class="sxs-lookup"><span data-stu-id="8c13f-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="8c13f-108">Fysisk besidder enheden bliver udslettet.</span><span class="sxs-lookup"><span data-stu-id="8c13f-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="8c13f-109">Kopier koden, før du udsteder sletningen.</span><span class="sxs-lookup"><span data-stu-id="8c13f-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="8c13f-110">**Bemærk:** Der er ikke store og små bogstaver i tørrekoden, så "-" tegnene er ikke påkrævet.</span><span class="sxs-lookup"><span data-stu-id="8c13f-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="8c13f-111">Yderligere oplysninger finder du [i Bypass Activation Lock on Supervised iOS-enheder med Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="8c13f-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="8c13f-112">**Ofte stillede spørgsmål**</span><span class="sxs-lookup"><span data-stu-id="8c13f-112">**FAQ**</span></span>

<span data-ttu-id="8c13f-113">Sp: **Jeg har udsendt en fjernhandling for at fjerne firmadata fra en enhed, og nu sidder den fast i en ventende tilstand.**</span><span class="sxs-lookup"><span data-stu-id="8c13f-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="8c13f-114">A: For en ekstern handling for at fuldføre, den målrettede enhed skal være online og sund.</span><span class="sxs-lookup"><span data-stu-id="8c13f-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="8c13f-115">I følgende situationer forbliver fjernhandlingen i ventende tilstand i 30 dage, eller indtil enheden anerkender kommandoen, når enheden:</span><span class="sxs-lookup"><span data-stu-id="8c13f-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="8c13f-116">Har ikke forbindelse.</span><span class="sxs-lookup"><span data-stu-id="8c13f-116">Does not have connectivity.</span></span>
- <span data-ttu-id="8c13f-117">Mister sin ledelsesstatus med Intune.</span><span class="sxs-lookup"><span data-stu-id="8c13f-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="8c13f-118">Hvis du mener, at en enhed ikke længere tjekker ind, og at den ikke fjerner firmadata, skal du vælge Slet.</span><span class="sxs-lookup"><span data-stu-id="8c13f-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="8c13f-119">Hvis du sletter enheden, fjernes enhedsposten, så den ikke længere vises på listen Intune over enheder.</span><span class="sxs-lookup"><span data-stu-id="8c13f-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="8c13f-120">Hvis enheden skal være aktiv igen, skal brugeren tilmelde enheden igen.</span><span class="sxs-lookup"><span data-stu-id="8c13f-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="8c13f-121">Sp: **Hvorfor er visse fjernhandlinger ikke tilgængelige for mig at bruge?**</span><span class="sxs-lookup"><span data-stu-id="8c13f-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="8c13f-122">A: Ikke alle platforme understøtter alle eksterne enhedshandlinger.</span><span class="sxs-lookup"><span data-stu-id="8c13f-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="8c13f-123">Følgende fjernhandlinger er platformsspecifikke.</span><span class="sxs-lookup"><span data-stu-id="8c13f-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="8c13f-124">Omgå aktiveringslås (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="8c13f-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="8c13f-125">Ny start (kun Windows)</span><span class="sxs-lookup"><span data-stu-id="8c13f-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="8c13f-126">Tilstanden Mistet (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="8c13f-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="8c13f-127">Find enhed (kun iOS)</span><span class="sxs-lookup"><span data-stu-id="8c13f-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="8c13f-128">Genstart (kun Windows)</span><span class="sxs-lookup"><span data-stu-id="8c13f-128">Restart (Windows only)</span></span>

<span data-ttu-id="8c13f-129">Du kan finde flere oplysninger om hver handling under [Tilgængelige enhedshandlinger](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="8c13f-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>