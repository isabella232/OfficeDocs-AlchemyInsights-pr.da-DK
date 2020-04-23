---
title: Fejlfinding i forbindelse med problemer med tilmelding af iOS-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736152"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="4e355-102">Fejlfinding i forbindelse med problemer med tilmelding af iOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4e355-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="4e355-103">Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="4e355-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4e355-104">Nogle almindelige fejlmeddelelser og løsningstrin:</span><span class="sxs-lookup"><span data-stu-id="4e355-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="4e355-105">**Enhedshætten er nået** Brugeren har flere enheder tilmeldt end enhedsgrænsen.</span><span class="sxs-lookup"><span data-stu-id="4e355-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4e355-106">Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="4e355-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="4e355-107">**Denne tjeneste understøttes ikke. Ingen tilmeldingspolitik:** Apns (Apple Push Notification Service) skal konfigureres eller fornys.</span><span class="sxs-lookup"><span data-stu-id="4e355-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="4e355-108">Gennemse [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få vejledning i, hvordan du gør det.</span><span class="sxs-lookup"><span data-stu-id="4e355-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="4e355-109">**Brugerlicenstypen Ugyldig eller brugernavn et ikke genkendt:** Brugeren skal tildeles en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="4e355-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4e355-110">Gennemse disse dokumenter for at tildele en licens via: [Office Administration](https://docs.microsoft.com/intune/licenses-assign) eller [Azure-portal .](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="4e355-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="4e355-111">Yderligere ressourcer, der kan hjælpe dig med at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="4e355-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4e355-112">Brug [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldingsfejl.</span><span class="sxs-lookup"><span data-stu-id="4e355-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4e355-113">Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="4e355-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4e355-114">Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsning af hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindingsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4e355-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="4e355-115">[Få mere at vide om, hvordan du tilmelder iOS-enheder i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="4e355-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

