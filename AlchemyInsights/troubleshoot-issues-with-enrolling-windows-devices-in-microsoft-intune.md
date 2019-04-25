---
title: Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390637"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="4c390-102">Fejlfinding i forbindelse med registreringen af Windows-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4c390-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="4c390-103">Gennemse ressourcerne nedenfor til at løse dit problem nu.</span><span class="sxs-lookup"><span data-stu-id="4c390-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4c390-104">Nogle almindelige fejlmeddelelser og trin opløsning:</span><span class="sxs-lookup"><span data-stu-id="4c390-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="4c390-105">**Kan ikke installeres softwaren, 0x80cf4017:** Din konto er udløbet.</span><span class="sxs-lookup"><span data-stu-id="4c390-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="4c390-106">Hent igen PC-klient softwarepakke i administrationskonsollen Intune.</span><span class="sxs-lookup"><span data-stu-id="4c390-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="4c390-107">Gennemse dokumentationen for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="4c390-107">Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="4c390-108">**Fejlkode 0x801c0003:** Fejlen kan opstå i følgende situationer:</span><span class="sxs-lookup"><span data-stu-id="4c390-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="4c390-109">Brugeren har flere enheder, der er tilmeldt end grænsen for enheden.</span><span class="sxs-lookup"><span data-stu-id="4c390-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4c390-110">Gennemgå disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre grænsen for enheden](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="4c390-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="4c390-111">"Brugere kan tilslutte enheder til Azure AD" er indstillet til "ingen".</span><span class="sxs-lookup"><span data-stu-id="4c390-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="4c390-112">Sæt den til alle, eller Vælg brugere.</span><span class="sxs-lookup"><span data-stu-id="4c390-112">Set it to all or select users.</span></span> <span data-ttu-id="4c390-113">Gennemse [dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="4c390-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="4c390-114">Enheden er allerede tilmeldt af en anden bruger.</span><span class="sxs-lookup"><span data-stu-id="4c390-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="4c390-115">Hvis det er tilfældet, kan du fjerne enheden fra konsollen Azure Intune eller manuelt unenroll enheden, før du prøver igen.</span><span class="sxs-lookup"><span data-stu-id="4c390-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="4c390-116">Enheden er Windows Home 10.</span><span class="sxs-lookup"><span data-stu-id="4c390-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="4c390-117">Kun Windows 10 Pro, uddannelse og Enterprise lagervarer kan deltage i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c390-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="4c390-118">Yderligere ressourcer til at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="4c390-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4c390-119">Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen.</span><span class="sxs-lookup"><span data-stu-id="4c390-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4c390-120">Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="4c390-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4c390-121">Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfinding doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="4c390-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="4c390-122">[Lær at registrere Windows-enheder i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="4c390-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

