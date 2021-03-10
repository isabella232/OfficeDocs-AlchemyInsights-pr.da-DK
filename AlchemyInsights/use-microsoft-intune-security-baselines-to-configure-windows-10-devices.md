---
title: Brug microsoft Intune-sikkerheds oprindelige planer til konfiguration af Windows 10-enheder
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50693414"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="e38df-102">Brug microsoft Intune-sikkerheds oprindelige planer til konfiguration af Windows 10-enheder</span><span class="sxs-lookup"><span data-stu-id="e38df-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="e38df-103">Intune-sikkerheds baselines hjælper med at beskytte brugere og enheder.</span><span class="sxs-lookup"><span data-stu-id="e38df-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="e38df-104">Sikkerheds baselines are Windows settings'pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span><span class="sxs-lookup"><span data-stu-id="e38df-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="e38df-105">Ved at oprette en profil for grundlinjer til sikkerhed i Intune kan du oprette en skabelon, der består af flere enhedskonfigurationsprofiler.</span><span class="sxs-lookup"><span data-stu-id="e38df-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="e38df-106">Når du installerer grundlinjer til sikkerhed for grupper af brugere eller enheder, anvendes indstillingerne på enheder, der kører på Windows 10 eller nyere versioner.</span><span class="sxs-lookup"><span data-stu-id="e38df-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="e38df-107">Sikkerheds baseline (1) for Microsoft Mobile Device Management (MDM) aktiverer f.eks. automatisk BitLocker til flytbare drev (2) kræver adgangskoden til åbning af en enhed, og (3) deaktiverer grundlæggende godkendelse.</span><span class="sxs-lookup"><span data-stu-id="e38df-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="e38df-108">Når en standardværdi ikke fungerer for dit miljø, kan du tilpasse den oprindelige plan for at anvende de indstillinger, du har brug for.</span><span class="sxs-lookup"><span data-stu-id="e38df-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="e38df-109">Sikkerheds baselines also help establish an end-to-end secure workflow in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e38df-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="e38df-110">Følgende er nogle af fordelene ved denne funktionalitet:</span><span class="sxs-lookup"><span data-stu-id="e38df-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="e38df-111">En grundlinje for sikkerhed omfatter de bedste fremgangsmåder og anbefalinger til indstillinger, der påvirker sikkerheden.</span><span class="sxs-lookup"><span data-stu-id="e38df-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="e38df-112">Da Intune samarbejder med Windows-sikkerhedsteamet, der opretter grundlinjer for gruppepolitikker, er disse anbefalinger baseret på solid vejledning og omfattende erfaring.</span><span class="sxs-lookup"><span data-stu-id="e38df-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="e38df-113">Hvis du er ny bruger af Intune og er usikker på, hvor du skal starte, kan sikkerheds oprindelige planer hjælpe dig med hurtigt at oprette og installere en sikker profil.</span><span class="sxs-lookup"><span data-stu-id="e38df-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="e38df-114">Hvis du i øjeblikket bruger en gruppepolitik, er det meget nemmere at overføre til Intune til administrationsformål med sikkerheds oprindelige planer, fordi disse sikkerheds oprindelige planer er indbygget i Intune og indeholder avancerede funktioner til administration.</span><span class="sxs-lookup"><span data-stu-id="e38df-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="e38df-115">Du kan finde flere oplysninger i [Windows-sikkerhedsscenarier](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [og administration af mobilenheder.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="e38df-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>