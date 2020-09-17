---
title: Fejlfinding af problemer med DEP-tilmelding i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797290"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="012e7-102">Fejlfinding af problemer med DEP-tilmelding i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="012e7-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="012e7-103">Gennemse de ressourcer, der er anført nedenfor, for at løse problemet nu.</span><span class="sxs-lookup"><span data-stu-id="012e7-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="012e7-104">Hvis DEP-enheden ikke kan registrere og MFA (multi-Factor Authentication) er aktiveret, skal du deaktivere MFA.</span><span class="sxs-lookup"><span data-stu-id="012e7-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="012e7-105">Aktuelt MFA understøttes ikke for registrering af forhindring af datakørsel</span><span class="sxs-lookup"><span data-stu-id="012e7-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="012e7-106">Brug [fejlfindings portalen til Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige tilmeldings fejl.</span><span class="sxs-lookup"><span data-stu-id="012e7-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="012e7-107">Gennemse [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="012e7-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="012e7-108">Gennemse disse dokumenter for at få en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver: [fejlfindingsvejledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfindings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="012e7-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="012e7-109">[Få mere at vide om tilmeldings programmet til enheder](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="012e7-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
