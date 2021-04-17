---
title: Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823457"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="d0522-102">Fejlfinding af problemer med registrering af iOS-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d0522-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="d0522-103">Gennemse ressourcerne nedenfor for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="d0522-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="d0522-104">Nogle almindelige fejlmeddelelser og løsningstrin:</span><span class="sxs-lookup"><span data-stu-id="d0522-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="d0522-105">**Caps til enhed er nået** Brugeren har flere enheder tilmeldt end enhedsgrænsen.</span><span class="sxs-lookup"><span data-stu-id="d0522-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d0522-106">Gennemse disse dokumenter for [at fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="d0522-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="d0522-107">**Denne tjeneste understøttes ikke. Ingen registreringspolitik:** Apple Push Notification Service (APNS) skal konfigureres eller fornyes.</span><span class="sxs-lookup"><span data-stu-id="d0522-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="d0522-108">Gennemgå [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få vejledning i, hvordan du gør dette.</span><span class="sxs-lookup"><span data-stu-id="d0522-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="d0522-109">**Brugerlicenstype Ugyldig eller Brugernavn blev ikke genkendt:** Brugeren skal have tildelt en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="d0522-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d0522-110">Gennemse disse dokumenter for at tildele en licens via: [Office Administration eller](https://docs.microsoft.com/intune/licenses-assign) [Azure-portalen](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="d0522-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="d0522-111">Yderligere ressourcer, der kan hjælpe med at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="d0522-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d0522-112">Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl.</span><span class="sxs-lookup"><span data-stu-id="d0522-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d0522-113">Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="d0522-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="d0522-114">Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger på hver enkelt: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [Fejlfinding af dokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="d0522-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="d0522-115">[Få mere at vide om, hvordan du tilmelder iOS-enheder i Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="d0522-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

