---
title: Fejlfinding af problemer med tilmelding af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759614"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="b7faf-102">Fejlfinding af problemer med tilmelding af Android-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b7faf-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="b7faf-103">Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="b7faf-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="b7faf-104">Nogle almindelige problemer og løsningstrin:</span><span class="sxs-lookup"><span data-stu-id="b7faf-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="b7faf-105">**Enheden er ikke krypteret i firmaportalen:** Nyere versioner af Android, især startende med v7.0, kræver en startadgangskode for at sikre, at din enhed er fuldt krypteret.</span><span class="sxs-lookup"><span data-stu-id="b7faf-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="b7faf-106">Almindelige løsninger er at aktivere en startpin eller kryptere enheden helt.</span><span class="sxs-lookup"><span data-stu-id="b7faf-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="b7faf-107">Gennemse [dette dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="b7faf-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="b7faf-108">**Enheder undlader at tjekke ind med Intune service eller vise som "Usundt" i Intune admin konsol:** Nogle Samsung 4.4- og 5.5-enheder tjekker muligvis ikke ind i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="b7faf-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="b7faf-109">Der er 3 mulige løsninger på dette problem:</span><span class="sxs-lookup"><span data-stu-id="b7faf-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="b7faf-110">Åbn intune-firmaportalappen manuelt, som automatisk starter en enhedssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="b7faf-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="b7faf-111">Opdater enheden til Android 6.0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="b7faf-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="b7faf-112">Deaktiver Samsung Smart Manager fra at administrere Intune Company Portal.</span><span class="sxs-lookup"><span data-stu-id="b7faf-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="b7faf-113">Læs [dette dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få yderligere oplysninger om disse spørgsmål og løsninger.</span><span class="sxs-lookup"><span data-stu-id="b7faf-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="b7faf-114">**Brugerlicenstype Ugyldig** eller **Fejl i brugernavnet ikke genkendt:** Brugeren skal tildeles en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="b7faf-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="b7faf-115">Gennemse disse dokumenter for at tildele en licens via: Office Administration eller Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="b7faf-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="b7faf-116">Yderligere ressourcer, der kan hjælpe dig med at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="b7faf-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b7faf-117">Brug [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldingsfejl.</span><span class="sxs-lookup"><span data-stu-id="b7faf-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="b7faf-118">Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="b7faf-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="b7faf-119">Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt.</span><span class="sxs-lookup"><span data-stu-id="b7faf-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="b7faf-120">[Få mere at vide om, hvordan du tilmelder Android-enheder i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="b7faf-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
