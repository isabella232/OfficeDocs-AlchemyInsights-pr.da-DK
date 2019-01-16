---
title: Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283251"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="b3f84-102">Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b3f84-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="b3f84-103">Gennemse ressourcerne nedenfor til at løse dit problem nu.</span><span class="sxs-lookup"><span data-stu-id="b3f84-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="b3f84-104">Nogle almindelige fejlmeddelelser og trin opløsning:</span><span class="sxs-lookup"><span data-stu-id="b3f84-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="b3f84-p101">**Kan ikke installeres softwaren, 0x80cf4017:** Din konto er udløbet. Hent igen PC-klient softwarepakke i administrationskonsollen Intune. Gennemse dokumentationen for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="b3f84-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="b3f84-108">**Fejlkode 0x801c0003:** Fejlen kan opstå i følgende situationer:</span><span class="sxs-lookup"><span data-stu-id="b3f84-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="b3f84-p102">Brugeren har flere enheder, der er tilmeldt end grænsen for enheden. Gennemgå disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/en-us/intune/devices-wipe) eller [ændre grænsen for enheden](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b3f84-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="b3f84-p103">"Brugere kan tilslutte enheder til Azure AD" er indstillet til "ingen". Sæt den til alle, eller Vælg brugere. Gennemse [dokumentationen](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="b3f84-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="b3f84-p104">Enheden er allerede tilmeldt af en anden bruger. Hvis det er tilfældet, kan du fjerne enheden fra konsollen Azure Intune eller manuelt unenroll enheden, før du prøver igen.</span><span class="sxs-lookup"><span data-stu-id="b3f84-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="b3f84-p105">Enheden er Windows Home 10. Kun Windows 10 Pro, uddannelse og Enterprise lagervarer kan deltage i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b3f84-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="b3f84-118">Yderligere ressourcer til at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="b3f84-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b3f84-p106">Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen. Gennemse [dette dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="b3f84-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b3f84-121">Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfinding doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b3f84-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="b3f84-122">[Lær at registrere Windows-enheder i Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="b3f84-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

