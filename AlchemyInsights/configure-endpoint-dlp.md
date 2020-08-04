---
title: Konfigurer DLP for slutpunkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555130"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="5f99c-102">Konfigurer DLP for slutpunkt</span><span class="sxs-lookup"><span data-stu-id="5f99c-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="5f99c-103">Microsoft Endpoint DLP giver dig mulighed for at udvide DLP-beskyttelse og overvågning til følsomme oplysninger på Windows 10-enheder.</span><span class="sxs-lookup"><span data-stu-id="5f99c-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="5f99c-104">Når enheder er indbygget i enhedsadministration, kan du oprette DLP-politikker for at gennemtvinge beskyttelseshandlinger for elementer.</span><span class="sxs-lookup"><span data-stu-id="5f99c-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="5f99c-105">Aktivitetsstifinder kan bruges til at overvåge aktivitet for følsomme elementer.</span><span class="sxs-lookup"><span data-stu-id="5f99c-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="5f99c-106">Du kan finde flere oplysninger under [Onboarding-enheder i enhedsadministration](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="5f99c-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="5f99c-107">Sådan kommer du i gang med DLP for slutpunkt:</span><span class="sxs-lookup"><span data-stu-id="5f99c-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="5f99c-108">Sørg for, at du har den relevante SKU/abonnementslicens.</span><span class="sxs-lookup"><span data-stu-id="5f99c-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="5f99c-109">Du kan finde flere oplysninger under [SKU/abonnementslicenser .](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)</span><span class="sxs-lookup"><span data-stu-id="5f99c-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="5f99c-110">Kontroller de tilladelser, der kræves for at aktivere enhedsadministration, få adgang til onboardingsiden eller aktivere overvågning af enheder til/fra.</span><span class="sxs-lookup"><span data-stu-id="5f99c-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="5f99c-111">Du kan finde flere oplysninger under [Tilladelser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="5f99c-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="5f99c-112">Indbyggede enheder i Enhedsadministration ved at følge onboardingudstyrsproceduren.</span><span class="sxs-lookup"><span data-stu-id="5f99c-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="5f99c-113">Hvis du mangler indstillingen Device Onboarding (preview) under M365 Compliance **Settings**, skal du bekræfte, at du har den relevante licens og de relevante tilladelser, der henvises til ovenfor.</span><span class="sxs-lookup"><span data-stu-id="5f99c-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="5f99c-114">Du kan finde flere oplysninger under [Onboarding-enheder](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="5f99c-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="5f99c-115">Opret DLP-politikker for at beskytte dine følsomme elementer.</span><span class="sxs-lookup"><span data-stu-id="5f99c-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="5f99c-116">Du kan finde flere oplysninger [under DLP-politikscenarier for slutpunkt.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)</span><span class="sxs-lookup"><span data-stu-id="5f99c-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="5f99c-117">Yderligere oplysninger om Microsoft Endpoint DLP finder du under [Få mere at vide om Microsoft 365-forebyggelse af datatab i slutpunkt (eksempel)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="5f99c-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>