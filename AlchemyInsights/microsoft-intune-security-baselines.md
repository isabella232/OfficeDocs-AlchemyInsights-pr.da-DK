---
title: Brug Microsoft Intune grundlinjer for sikkerhed til at konfigurere Windows 10 enheder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793612"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="59922-102">Brug Microsoft Intune grundlinjer for sikkerhed til at konfigurere Windows 10 enheder</span><span class="sxs-lookup"><span data-stu-id="59922-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="59922-103">Intune-sikkerheds oprindelige planer hjælper med at beskytte brugere og enheder.</span><span class="sxs-lookup"><span data-stu-id="59922-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="59922-104">Grundlinjer for sikkerhed er Windows forudkonfigurerede grupper, der bruges til at anvende en kendt gruppe af indstillinger og standardværdier anbefalet af de relevante sikkerhedsteams.</span><span class="sxs-lookup"><span data-stu-id="59922-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="59922-105">Ved at oprette en profil for grundlinjer for sikkerheden i Intune kan du oprette en skabelon, der består af flere enhedskonfigurationsprofiler.</span><span class="sxs-lookup"><span data-stu-id="59922-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="59922-106">Når du installerer grundlinjer for sikkerhed for grupper af brugere eller enheder, anvendes indstillingerne på enheder, der kører på Windows 10 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="59922-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="59922-107">Sikkerheds baseline for Microsoft mobile device management (MDM) aktiverer f.eks. automatisk BitLocker til flytbare drev, kræver adgangskoden til at låse en enhed op og deaktiverer grundlæggende godkendelse.</span><span class="sxs-lookup"><span data-stu-id="59922-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="59922-108">Når en standardværdi ikke fungerer for dit miljø, kan du tilpasse den oprindelige plan for at anvende de indstillinger, du har brug for.</span><span class="sxs-lookup"><span data-stu-id="59922-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="59922-109">Sikkerheds oprindelige planer hjælper også med at oprette en en sikker arbejdsproces i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="59922-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="59922-110">En grundlinje for sikkerhed indeholder de bedste fremgangsmåder og anbefalinger til indstillinger, der påvirker sikkerheden.</span><span class="sxs-lookup"><span data-stu-id="59922-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="59922-111">Intune arbejder sammen med Windows, der opretter oprindelige planer for gruppepolitikker, så disse anbefalinger er baseret på solid vejledning og omfattende erfaring.</span><span class="sxs-lookup"><span data-stu-id="59922-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="59922-112">Hvis du er ny bruger af Intune og er usikker på, hvor du skal starte, hjælper sikkerheds oprindelige planer dig med hurtigt at oprette og implementere en sikker profil.</span><span class="sxs-lookup"><span data-stu-id="59922-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="59922-113">Hvis du aktuelt bruger en gruppepolitik, er det meget nemmere at overføre til Intune til administrationsformål med sikkerheds oprindelige planer, fordi de er indbygget i Intune og indeholder avancerede administrationsfunktioner.</span><span class="sxs-lookup"><span data-stu-id="59922-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="59922-114">Du kan få mere at vide [Windows sikkerheds oprindelige planer](/windows/security/threat-protection/windows-security-baselines) og Administration af [mobilenheder.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="59922-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

