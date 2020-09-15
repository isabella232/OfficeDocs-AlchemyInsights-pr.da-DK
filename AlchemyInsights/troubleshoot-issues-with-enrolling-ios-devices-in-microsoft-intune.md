---
title: Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669242"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="c48b2-102">Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c48b2-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="c48b2-103">Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="c48b2-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c48b2-104">Nogle almindelige fejlmeddelelser og løsnings trin:</span><span class="sxs-lookup"><span data-stu-id="c48b2-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="c48b2-105">**Enheds dæksel er nået** Brugeren har flere enheder, der er tilmeldt en enheds grænse.</span><span class="sxs-lookup"><span data-stu-id="c48b2-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c48b2-106">Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre enheds grænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="c48b2-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="c48b2-107">**Denne tjeneste understøttes ikke. Ingen registreringspolitik:** Apple Push Notification-tjenesten (APNS) skal være konfigureret eller fornyet.</span><span class="sxs-lookup"><span data-stu-id="c48b2-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="c48b2-108">Gennemgå [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få oplysninger om, hvordan du gør det.</span><span class="sxs-lookup"><span data-stu-id="c48b2-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="c48b2-109">**Brugerlicens typen er ugyldig, eller brugernavnet blev ikke genkendt:** Brugeren skal have tildelt en Intune-eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="c48b2-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c48b2-110">Gennemgå disse dokumenter for at tildele en licens via: [Office administration](https://docs.microsoft.com/intune/licenses-assign) eller [Azure-portalen](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="c48b2-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="c48b2-111">Yderligere ressourcer, der kan hjælpe med at løse dit problem:</span><span class="sxs-lookup"><span data-stu-id="c48b2-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c48b2-112">Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl.</span><span class="sxs-lookup"><span data-stu-id="c48b2-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c48b2-113">Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="c48b2-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c48b2-114">Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver: [fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c48b2-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="c48b2-115">[Få mere at vide om, hvordan du registrerer iOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="c48b2-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

