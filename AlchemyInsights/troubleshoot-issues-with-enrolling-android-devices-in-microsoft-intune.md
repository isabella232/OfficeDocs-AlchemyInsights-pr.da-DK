---
title: Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689948"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="8b7f1-102">Fejlfinding af problemer med registrering af Android-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8b7f1-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="8b7f1-103">Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="8b7f1-104">Nogle almindelige problemer og løsnings trin:</span><span class="sxs-lookup"><span data-stu-id="8b7f1-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="8b7f1-105">**Enheden har ikke en krypteret fejl i firmaportalen:** Nyere versioner af Android, især fra og med v 7.0, kræver en start adgangskode for at sikre, at enheden er fuldt krypteret.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="8b7f1-106">Almindelige løsninger er at aktivere en startpinkode eller en fuldt krypteret enhed.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="8b7f1-107">Gennemse [dette dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="8b7f1-108">Det **lykkedes ikke at tjekke enheder ind med tjenesten Intune eller Vis som "usund" i Intune-administrationskonsollen:** Nogle Samsung 4,4-og 5,5-enheder kan muligvis ikke tjekkes ind i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="8b7f1-109">Der er 3 mulige løsninger på dette problem:</span><span class="sxs-lookup"><span data-stu-id="8b7f1-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="8b7f1-110">Åbn appen Intune-Firmaportalen manuelt, der starter automatisk en enhedssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="8b7f1-111">Opdater enheden til Android 6,0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="8b7f1-112">Deaktiver Samsung Smart Manager fra at administrere Intune-Firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="8b7f1-113">Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få flere oplysninger om disse problemer og løsninger.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="8b7f1-114">**Brugerlicens typen er ugyldig** , eller **brugernavnet blev ikke genkendt fejlen:** brugeren skal have tildelt en Intune-eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="8b7f1-115">Gennemgå disse dokumenter for at tildele en licens via: Office administration eller Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="8b7f1-116">Yderligere ressourcer, der kan hjælpe med at løse dit problem:</span><span class="sxs-lookup"><span data-stu-id="8b7f1-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="8b7f1-117">Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8b7f1-118">Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="8b7f1-119">Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for at få en liste over almindelige fejl, der forhindrer registrering og løsninger til hver enkelt.</span><span class="sxs-lookup"><span data-stu-id="8b7f1-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="8b7f1-120">[Få mere at vide om, hvordan du registrerer Android-enheder i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="8b7f1-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
