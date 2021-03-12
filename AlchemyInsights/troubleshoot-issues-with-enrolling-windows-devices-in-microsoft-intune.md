---
title: Fejlfinding af problemer med tilmelding af Windows-enheder i Microsoft Intune
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708884"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="3817a-102">Fejlfinding af problemer med tilmelding af Windows-enheder i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3817a-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="3817a-103">Gennemse ressourcerne nedenfor for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="3817a-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="3817a-104">Nogle almindelige fejlmeddelelser og løsningstrin:</span><span class="sxs-lookup"><span data-stu-id="3817a-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="3817a-105">**Softwaren kan ikke installeres, 0x80cf4017:** Dit kontocertifikat er udløbet.</span><span class="sxs-lookup"><span data-stu-id="3817a-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="3817a-106">Hent pc-klientsoftwarepakken igen i Intune-administrationskonsollen.</span><span class="sxs-lookup"><span data-stu-id="3817a-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="3817a-107">Gennemgå denne dokumentation for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="3817a-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="3817a-108">**Fejlkode 0x801c0003:** Fejlen kan opstå i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="3817a-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="3817a-109">Brugeren har flere enheder tilmeldt end enhedsgrænsen.</span><span class="sxs-lookup"><span data-stu-id="3817a-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3817a-110">Gennemse disse dokumenter for [at fjerne en enhed](https://docs.microsoft.com/intune/devices-wipe) eller ændre [enhedsgrænsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="3817a-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="3817a-111">"Brugere kan slutte enheder til Azure AD" er indstillet til "ingen".</span><span class="sxs-lookup"><span data-stu-id="3817a-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="3817a-112">Indstil den til alle eller vælg brugere.</span><span class="sxs-lookup"><span data-stu-id="3817a-112">Set it to all or select users.</span></span> <span data-ttu-id="3817a-113">Gennemgå [denne dokumentation for](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="3817a-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="3817a-114">Enheden er allerede tilmeldt af en anden bruger.</span><span class="sxs-lookup"><span data-stu-id="3817a-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="3817a-115">Hvis det er tilfældet, skal du fjerne enheden fra Azure Intune-konsollen eller manuelt fjerne tilmeldingen af enheden, før du prøver igen.</span><span class="sxs-lookup"><span data-stu-id="3817a-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="3817a-116">Enheden er Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="3817a-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="3817a-117">Kun Windows 10 Pro-, Education- og Enterprise SKU'er kan deltage i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3817a-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="3817a-118">Yderligere ressourcer til at løse problemet:</span><span class="sxs-lookup"><span data-stu-id="3817a-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="3817a-119">Brug [Intune-fejlfindingsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige registreringsfejl.</span><span class="sxs-lookup"><span data-stu-id="3817a-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3817a-120">Gennemgå [dette dokument for](https://docs.microsoft.com/intune/help-desk-operators) at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="3817a-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="3817a-121">Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer registrering og løsninger til hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [fejlfindingsdokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="3817a-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="3817a-122">[Få mere at vide om, hvordan du tilmelder Windows-enheder i Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="3817a-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
