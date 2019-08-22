---
title: Fejlfinding i forbindelse med tilmelding til forhindring af Datakørsel i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 3e10f6729d760d9f8f6d04bcb33317fde51a9b80
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506872"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="868c3-102">Fejlfinding i forbindelse med tilmelding til forhindring af Datakørsel i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="868c3-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="868c3-103">Gennemse ressourcerne nedenfor til at løse dit problem nu.</span><span class="sxs-lookup"><span data-stu-id="868c3-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="868c3-104">Hvis Forhindring af Datakørsel enhed kan ikke tilmeldes og MFA (godkendelse i flere niveauer) er aktiveret, skal du deaktivere MFA.</span><span class="sxs-lookup"><span data-stu-id="868c3-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="868c3-105">I øjeblikket understøttes MFA ikke for Forhindring af Datakørsel tilmelding</span><span class="sxs-lookup"><span data-stu-id="868c3-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="868c3-106">Bruge [Intune fejlfinding Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til at diagnosticere og løse almindelige fejl i registreringen.</span><span class="sxs-lookup"><span data-stu-id="868c3-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="868c3-107">Gennemse [dette dokument](https://docs.microsoft.com/intune/help-desk-operators) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="868c3-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="868c3-108">Gennemgå disse dokumenter for en liste over almindelige fejl, der forhindrer tilmelding og løsninger til hver enkelt: [vejledning til fejlfinding](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [fejlfinding doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="868c3-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="868c3-109">[Få mere at vide om programmet til enheden for tilmelding](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="868c3-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
