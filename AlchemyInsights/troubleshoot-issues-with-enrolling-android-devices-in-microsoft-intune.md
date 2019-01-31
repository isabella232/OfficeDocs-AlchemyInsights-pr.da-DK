---
title: Fejlfinding i forbindelse med registreringen af Android-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655877"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="aa0cd-102">Fejlfinding i forbindelse med registreringen af Android-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="aa0cd-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="aa0cd-103">Gennemse ressourcerne nedenfor til at løse dit problem nu.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="aa0cd-104">Nogle almindelige problemer og trin til løsning:</span><span class="sxs-lookup"><span data-stu-id="aa0cd-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="aa0cd-p101">**Enhed ikke krypteret fejl i firmaets Portal:** Nyere versioner af Android, især fra og med v7.0, kræver en start-adgangskode til at sikre, at enheden bliver fuldt krypteret. Almindelige løsninger er at aktivere pinkoden start eller fuldt krypterer enheden. Gennemse [dette dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="aa0cd-p102">**Enheder ikke kan kontrollere med tjenesten Intune eller vises som "Unhealthy" i administrationskonsollen Intune:** Nogle Samsung 4.4 og 5.5 enheder kan ikke kontrollere på tjenesten. Der er 3 mulige løsninger på dette problem:</span><span class="sxs-lookup"><span data-stu-id="aa0cd-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="aa0cd-110">Åbn app Intune firmaets Portal, som automatisk starter en enhedssynkronisering manuelt.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="aa0cd-111">Opdatere enheden Android 6.0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="aa0cd-p103">Du kan deaktivere Samsung Smart Manager fra administration af portalen Intune virksomhed. Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for at få yderligere oplysninger om disse problemer og løsninger.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="aa0cd-p104">**Bruger licens Type ugyldige** eller **bruger navn blev ikke genkendt fejl:** brugeren skal være tildelt en licens til Intune eller EMS. Gennemgå disse dokumenter for at tildele en licens til: Office Admin Center eller Azure portal.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="aa0cd-116">Yderligere ressourcer til at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="aa0cd-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="aa0cd-p105">Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen. Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="aa0cd-119">Gennemse [dette dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver.</span><span class="sxs-lookup"><span data-stu-id="aa0cd-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="aa0cd-120">[Lær at tilmelde Android-enheder i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="aa0cd-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

