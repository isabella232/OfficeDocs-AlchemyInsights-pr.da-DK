---
title: Fejlfinding i forbindelse med registrering af Windows-enheder i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665826"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="725c7-102">Fejlfinding i forbindelse med registrering af Windows-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="725c7-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="725c7-103">Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="725c7-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="725c7-104">Nogle almindelige fejlmeddelelser og løsningstrin:</span><span class="sxs-lookup"><span data-stu-id="725c7-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="725c7-105">**Softwaren kan ikke installeres, 0x80cf4017:** Dit kontocertifikat er udløbet.</span><span class="sxs-lookup"><span data-stu-id="725c7-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="725c7-106">Download pc-klientens softwarepakke igen i Intune Admin Console.</span><span class="sxs-lookup"><span data-stu-id="725c7-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="725c7-107">Læs denne dokumentation for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="725c7-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="725c7-108">**Fejlkode 0x801c0003:** Fejlen kan opstå i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="725c7-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="725c7-109">Brugeren har flere enheder tilmeldt end enhedsgrænsen.</span><span class="sxs-lookup"><span data-stu-id="725c7-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="725c7-110">Gennemse disse dokumenter for at [fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="725c7-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="725c7-111">"Brugere kan slutte sig til azure AD" er indstillet til "ingen".</span><span class="sxs-lookup"><span data-stu-id="725c7-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="725c7-112">Indstil den til alle eller vælg brugere.</span><span class="sxs-lookup"><span data-stu-id="725c7-112">Set it to all or select users.</span></span> <span data-ttu-id="725c7-113">Læs [denne dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="725c7-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="725c7-114">Enheden er allerede tilmeldt af en anden bruger.</span><span class="sxs-lookup"><span data-stu-id="725c7-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="725c7-115">Hvis det er tilfældet, skal du fjerne enheden fra Azure Intune-konsollen eller manuelt frigøre enheden, før du prøver igen.</span><span class="sxs-lookup"><span data-stu-id="725c7-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="725c7-116">Enheden er Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="725c7-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="725c7-117">Det er kun Windows 10 Pro- og Education- og Enterprise-SKU'er, der kan deltage i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="725c7-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="725c7-118">Yderligere ressourcer, der kan hjælpe dig med at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="725c7-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="725c7-119">Brug [Intune-fejlfindingsportal til](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) at diagnosticere og løse almindelige tilmeldingsfejl.</span><span class="sxs-lookup"><span data-stu-id="725c7-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="725c7-120">Læs [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="725c7-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="725c7-121">Gennemse disse dokumenter for at få vist en liste over almindelige fejl, der forhindrer tilmelding og løsninger på de enkelte: [Fejlfindingsvejledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [Fejlfinding af dokumenter](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="725c7-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="725c7-122">[Få mere at vide om, hvordan du tilmelder Windows-enheder i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="725c7-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
