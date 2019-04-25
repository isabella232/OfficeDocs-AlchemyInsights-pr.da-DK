---
title: Fejlfinding i forbindelse med registreringen af iOS enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391001"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="cb075-102">Fejlfinding i forbindelse med registreringen af iOS enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cb075-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="cb075-103">Gennemse ressourcerne nedenfor til at løse dit problem nu.</span><span class="sxs-lookup"><span data-stu-id="cb075-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="cb075-104">Nogle almindelige fejlmeddelelser og trin opløsning:</span><span class="sxs-lookup"><span data-stu-id="cb075-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="cb075-105">**Enheden Cap er nået** Brugeren har flere enheder, der er tilmeldt end grænsen for enheden.</span><span class="sxs-lookup"><span data-stu-id="cb075-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="cb075-106">Gennemgå disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre grænsen for enheden](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="cb075-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="cb075-107">**Denne Service er ikke understøttet. Ingen registreringspolitik:** Apple Push Notification Service (APN'ER) skal være konfigureret eller fornyes.</span><span class="sxs-lookup"><span data-stu-id="cb075-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="cb075-108">Gennemse [dette dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for at få instruktioner om, hvordan du gør det.</span><span class="sxs-lookup"><span data-stu-id="cb075-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="cb075-109">**Bruger licens Type ugyldige eller brugernavn blev ikke genkendt:** Brugeren skal være tildelt en licens til Intune eller EMS.</span><span class="sxs-lookup"><span data-stu-id="cb075-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="cb075-110">Gennemgå disse dokumenter for at tildele en licens til: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="cb075-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="cb075-111">Yderligere ressourcer til at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="cb075-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="cb075-112">Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen.</span><span class="sxs-lookup"><span data-stu-id="cb075-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="cb075-113">Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="cb075-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="cb075-114">Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfinding doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="cb075-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="cb075-115">[Lær, hvordan du registrere iOS enheder i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="cb075-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

