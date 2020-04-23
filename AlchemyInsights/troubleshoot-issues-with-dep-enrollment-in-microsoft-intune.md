---
title: Fejlfinding i forbindelse med problemer med tilmelding til forhindring af datap i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 11b0d73c34996fd84431b38d77b64536d386977e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766703"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="92fbf-102">Fejlfinding i forbindelse med problemer med tilmelding til forhindring af datap i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="92fbf-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="92fbf-103">Gennemgå de ressourcer, der er angivet nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="92fbf-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="92fbf-104">Hvis Forhindring af datap-enhed ikke kan tilmelde sig, og MFA (Multi-Factor Authentication) er aktiveret, skal du deaktivere MFA.</span><span class="sxs-lookup"><span data-stu-id="92fbf-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="92fbf-105">I øjeblikket understøttes MFA ikke ved tilmelding af forhindring af datap</span><span class="sxs-lookup"><span data-stu-id="92fbf-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="92fbf-106">Brug [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldingsfejl.</span><span class="sxs-lookup"><span data-stu-id="92fbf-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="92fbf-107">Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="92fbf-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="92fbf-108">Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsning af hver: [Fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindingsvejledning](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="92fbf-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="92fbf-109">[Få mere at vide om programmet til tilmelding af enheder](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="92fbf-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
