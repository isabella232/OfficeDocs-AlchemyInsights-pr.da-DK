---
title: Brug sikkerhedsplaner for Microsoft Intune til at konfigurere Windows 10-enheder
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573331"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="4b677-102">Brug sikkerhedsplaner for Microsoft Intune til at konfigurere Windows 10-enheder</span><span class="sxs-lookup"><span data-stu-id="4b677-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="4b677-103">Intune-sikkerhedsplaner hjælper med at beskytte brugere og enheder.</span><span class="sxs-lookup"><span data-stu-id="4b677-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="4b677-104">Sikkerhedsplaner er Windows-indstillinger ' forudkonfigurerede grupper, der bruges til at anvende en kendt gruppe af indstillinger og standardværdier, der anbefales af de relevante sikkerheds teams.</span><span class="sxs-lookup"><span data-stu-id="4b677-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="4b677-105">Hvis du opretter en oprindelig plan for oprindelige profiler i Intune, opretter du en skabelon, der består af flere enheds konfigurationsprofiler.</span><span class="sxs-lookup"><span data-stu-id="4b677-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="4b677-106">Når du installerer sikkerhedsplaner til grupper af brugere eller enheder, anvendes indstillingerne på enheder, der kører på Windows 10 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="4b677-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="4b677-107">For eksempel gør MDM-sikkerheds grundlinje automatisk (1) aktiverer BitLocker for flytbare drev, (2) kræver adgangskoden til at låse en enhed op, og (3) deaktiverer grundlæggende godkendelse.</span><span class="sxs-lookup"><span data-stu-id="4b677-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="4b677-108">Når en standardværdi ikke fungerer for dit miljø, kan du tilpasse grundlinjen for at anvende de ønskede indstillinger.</span><span class="sxs-lookup"><span data-stu-id="4b677-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="4b677-109">Sikkerhedsplaner hjælper også med at oprette en slut-til-slut-arbejdsproces i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4b677-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="4b677-110">Følgende er nogle fordele ved dette:</span><span class="sxs-lookup"><span data-stu-id="4b677-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="4b677-111">En sikkerheds basis omfatter de bedste fremgangsmåder og anbefalinger til indstillinger, der påvirker sikkerheden.</span><span class="sxs-lookup"><span data-stu-id="4b677-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="4b677-112">Da Intune-partnere med Windows-sikkerheds teamet, der opretter grundlinjer til gruppepolitikker, er disse anbefalinger baseret på en dækkende vejledning og en omfattende oplevelse.</span><span class="sxs-lookup"><span data-stu-id="4b677-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="4b677-113">Hvis du er ny bruger af Intune og ikke er sikker på, hvor du skal starte, kan du bruge sikkerhedsplaner til hurtigt at oprette og installere en sikker profil.</span><span class="sxs-lookup"><span data-stu-id="4b677-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="4b677-114">Hvis du i øjeblikket bruger en gruppepolitik, er det meget nemmere at overføre til Intune til administrationsformål, fordi de er indbygget i Intune og omfatter de allernyeste funktioner til administration.</span><span class="sxs-lookup"><span data-stu-id="4b677-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="4b677-115">Hvis du vil have mere at vide, skal du se [Windows-sikkerhedsplaner](https://go.microsoft.com/fwlink/?linkid=2141503) og [administration af mobilenheder](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="4b677-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>