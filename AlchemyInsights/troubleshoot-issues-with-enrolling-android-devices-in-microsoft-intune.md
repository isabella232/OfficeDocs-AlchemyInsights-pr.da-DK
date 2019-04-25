---
title: Fejlfinding i forbindelse med registreringen af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420586"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="7c3bc-102">Fejlfinding i forbindelse med registreringen af Android-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7c3bc-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="7c3bc-103">Gennemse ressourcerne nedenfor til at løse dit problem nu.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="7c3bc-104">Nogle almindelige problemer og trin til løsning:</span><span class="sxs-lookup"><span data-stu-id="7c3bc-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="7c3bc-105">**Enhed ikke krypteret fejl i firmaets Portal:** Nyere versioner af Android, især fra og med v7.0, kræver en start-adgangskode til at sikre, at enheden bliver fuldt krypteret.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="7c3bc-106">Almindelige løsninger er at aktivere pinkoden start eller fuldt krypterer enheden.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="7c3bc-107">Gennemse [dette dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="7c3bc-108">**Enheder ikke kan kontrollere med tjenesten Intune eller vises som "Unhealthy" i administrationskonsollen Intune:** Nogle Samsung 4.4 og 5.5 enheder kan ikke kontrollere på tjenesten.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="7c3bc-109">Der er 3 mulige løsninger på dette problem:</span><span class="sxs-lookup"><span data-stu-id="7c3bc-109">There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="7c3bc-110">Åbn app Intune firmaets Portal, som automatisk starter en enhedssynkronisering manuelt.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="7c3bc-111">Opdatere enheden Android 6.0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="7c3bc-112">Du kan deaktivere Samsung Smart Manager fra administration af portalen Intune virksomhed.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="7c3bc-113">Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få yderligere oplysninger om disse problemer og løsninger.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="7c3bc-114">**Bruger licens Type ugyldige** eller **bruger navn blev ikke genkendt fejl:** brugeren skal være tildelt en licens til Intune eller EMS.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="7c3bc-115">Gennemgå disse dokumenter for at tildele en licens til: Office Admin Center eller Azure portal.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="7c3bc-116">Yderligere ressourcer til at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="7c3bc-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="7c3bc-117">Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="7c3bc-118">Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="7c3bc-119">Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver.</span><span class="sxs-lookup"><span data-stu-id="7c3bc-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="7c3bc-120">[Lær at tilmelde Android-enheder i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="7c3bc-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

