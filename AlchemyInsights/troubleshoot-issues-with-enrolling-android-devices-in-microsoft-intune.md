---
title: Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830936"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="a05a8-102">Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a05a8-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="a05a8-103">Gennemse ressourcerne nedenfor for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="a05a8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a05a8-104">Nogle almindelige problemer og løsningstrin:</span><span class="sxs-lookup"><span data-stu-id="a05a8-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="a05a8-105">**Fejlen Enhed er ikke krypteret i firmaportalen:** Nyere versioner af Android, især fra og med v7.0, kræver en start-adgangskode for at sikre, at enheden er fuldt krypteret.</span><span class="sxs-lookup"><span data-stu-id="a05a8-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="a05a8-106">Almindelige løsninger er at aktivere en startpinkode eller kryptere enheden fuldt ud.</span><span class="sxs-lookup"><span data-stu-id="a05a8-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="a05a8-107">Gennemgå [dette dokument for at](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="a05a8-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="a05a8-108">**Enheder kan ikke tjekke ind med Intune-tjenesten eller vises som "Usunde" i Intune-administrationskonsollen:** Nogle Samsung 4.4- og 5.5-enheder kan ikke tjekke ind i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="a05a8-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="a05a8-109">Der er tre mulige løsninger på dette problem:</span><span class="sxs-lookup"><span data-stu-id="a05a8-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="a05a8-110">Åbn appen Intune-firmaportal manuelt, som automatisk starter en enhedssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="a05a8-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="a05a8-111">Opdater enheden til Android 6.0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="a05a8-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="a05a8-112">Deaktiver Samsung Smart Manager fra at administrere Intune-firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="a05a8-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="a05a8-113">Gennemgå [dette dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få flere oplysninger om disse problemer og løsninger.</span><span class="sxs-lookup"><span data-stu-id="a05a8-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="a05a8-114">**Fejlen Brugerlicenstype** Ugyldig **eller Brugernavn genkendes ikke:** Brugeren skal have tildelt en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="a05a8-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="a05a8-115">Gennemse disse dokumenter for at tildele en licens via: Office Administration eller Azure-portal.</span><span class="sxs-lookup"><span data-stu-id="a05a8-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="a05a8-116">Yderligere ressourcer, der kan hjælpe med at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="a05a8-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="a05a8-117">Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl.</span><span class="sxs-lookup"><span data-stu-id="a05a8-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a05a8-118">Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="a05a8-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="a05a8-119">Gennemgå [dette dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for at få en liste over almindelige fejl, der forhindrer registrering og løsninger på hver enkelt.</span><span class="sxs-lookup"><span data-stu-id="a05a8-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="a05a8-120">[Få mere at vide om, hvordan du tilmelder Android-enheder i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="a05a8-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
