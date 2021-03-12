---
title: Fejlfinding af problemer med tilmelding af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708992"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="80e61-102">Fejlfinding af problemer med tilmelding af Android-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="80e61-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="80e61-103">Gennemse ressourcerne nedenfor for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="80e61-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="80e61-104">Nogle almindelige problemer og løsningstrin:</span><span class="sxs-lookup"><span data-stu-id="80e61-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="80e61-105">**Fejl i forbindelse med ikke-krypteret enhed i Firmaportal:** Nyere versioner af Android, især fra og med v7.0, kræver en start adgangskode for at sikre, at enheden er fuldt krypteret.</span><span class="sxs-lookup"><span data-stu-id="80e61-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="80e61-106">Almindelige løsninger er at aktivere en startpinkode eller kryptere enheden fuldt ud.</span><span class="sxs-lookup"><span data-stu-id="80e61-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="80e61-107">Gennemse [dette dokument for](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="80e61-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="80e61-108">**Enheder kan ikke tjekke ind med Intune-tjenesten eller vises som "Usund" i Intune-administrationskonsollen:** Nogle Samsung 4.4- og 5.5-enheder kontrollerer muligvis ikke tjenesten.</span><span class="sxs-lookup"><span data-stu-id="80e61-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="80e61-109">Der er tre mulige løsninger på dette problem:</span><span class="sxs-lookup"><span data-stu-id="80e61-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="80e61-110">Åbn appen Intune-firmaportal manuelt, som automatisk starter en enhedssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="80e61-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="80e61-111">Opdater enheden til Android 6.0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="80e61-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="80e61-112">Deaktiver Samsung Smart Manager fra at administrere Intune-firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="80e61-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="80e61-113">Gennemgå [dette dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få flere oplysninger om disse problemer og løsninger.</span><span class="sxs-lookup"><span data-stu-id="80e61-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="80e61-114">**Fejlen Ugyldig brugerlicens** **eller Brugernavn blev ikke genkendt:** Brugeren skal have tildelt en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="80e61-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="80e61-115">Gennemse disse dokumenter for at tildele en licens via: Office Administration eller Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="80e61-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="80e61-116">Yderligere ressourcer til at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="80e61-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="80e61-117">Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl.</span><span class="sxs-lookup"><span data-stu-id="80e61-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="80e61-118">Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="80e61-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="80e61-119">Gennemse [dette dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for at få en liste over almindelige fejl, der forhindrer registrering og løsninger på hver enkelt.</span><span class="sxs-lookup"><span data-stu-id="80e61-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="80e61-120">[Få mere at vide om, hvordan du tilmelder Android-enheder i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="80e61-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
