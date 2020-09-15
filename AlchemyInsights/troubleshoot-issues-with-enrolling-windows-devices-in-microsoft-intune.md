---
title: Fejlfinding af problemer med registrering af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658872"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="9f5e4-102">Fejlfinding af problemer med registrering af Windows-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9f5e4-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="9f5e4-103">Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9f5e4-104">Nogle almindelige fejlmeddelelser og løsnings trin:</span><span class="sxs-lookup"><span data-stu-id="9f5e4-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="9f5e4-105">**Softwaren kan ikke installeres, 0x80cf4017:** Dit konto certifikat er udløbet.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="9f5e4-106">Download PC-klientsoftware pakken igen i Intune-administrationskonsollen.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="9f5e4-107">Læs denne dokumentation for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="9f5e4-108">**Fejlkode 0x801c0003:** Fejlen kan forekomme i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="9f5e4-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="9f5e4-109">Brugeren har flere enheder, der er tilmeldt en enheds grænse.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9f5e4-110">Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller [ændre enheds grænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="9f5e4-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="9f5e4-111">"Brugerne kan tilmelde sig enheder til Azure AD" er indstillet til "ingen".</span><span class="sxs-lookup"><span data-stu-id="9f5e4-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="9f5e4-112">Sæt det til alle, eller Vælg brugere.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-112">Set it to all or select users.</span></span> <span data-ttu-id="9f5e4-113">Læs [denne dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="9f5e4-114">Enheden er allerede tilmeldt en anden bruger.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="9f5e4-115">Hvis det er tilfældet, skal du fjerne enheden fra Azure Intune-konsollen eller fjerne registreringen af enheden manuelt, før du prøver igen.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="9f5e4-116">Enheden er Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="9f5e4-117">Kun Windows 10 Pro-, Education-og Enterprise-SKU'er kan deltage i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="9f5e4-118">Yderligere ressourcer, der kan hjælpe med at løse dit problem:</span><span class="sxs-lookup"><span data-stu-id="9f5e4-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="9f5e4-119">Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9f5e4-120">Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="9f5e4-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="9f5e4-121">Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver: [fejlfindingsvejledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfindings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9f5e4-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="9f5e4-122">[Få mere at vide om, hvordan du tilmelder Windows-enheder i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="9f5e4-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
