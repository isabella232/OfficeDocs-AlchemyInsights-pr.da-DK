---
title: Konfigurer Slutpunkt DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402410"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="700d9-102">Konfigurer Slutpunkt DLP</span><span class="sxs-lookup"><span data-stu-id="700d9-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="700d9-103">Microsoft Slutpunkt DLP giver dig mulighed at udvide DLP-beskyttelse og overvågning til følsomme oplysninger på Windows 10-enheder.</span><span class="sxs-lookup"><span data-stu-id="700d9-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="700d9-104">Når enheder er integreret i enhedsstyring, kan du oprette DLP-politikker for at gennemtvinge beskyttende handlinger for elementer.</span><span class="sxs-lookup"><span data-stu-id="700d9-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="700d9-105">Aktivitetsoversigten kan bruges til at overvåge aktivitet for følsomme elementer.</span><span class="sxs-lookup"><span data-stu-id="700d9-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="700d9-106">Du kan få mere at vide under [Tilføjelse af enheder til enhedsstyring](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="700d9-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="700d9-107">Sådan kommer du i gang med Slutpunkt DLP:</span><span class="sxs-lookup"><span data-stu-id="700d9-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="700d9-108">Sørg for, at du har den rette SKU/abonnementslicens.</span><span class="sxs-lookup"><span data-stu-id="700d9-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="700d9-109">Du kan finde flere oplysninger i[Licenser til SKU/abonnementer](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="700d9-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="700d9-110">Kontrollér de tilladelser, der kræves for at aktivere enhedsstyring, få adgang til onboarding-siden eller aktivere/deaktivere overvågning af enheder.</span><span class="sxs-lookup"><span data-stu-id="700d9-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="700d9-111">Du kan finde flere oplysninger under [Tilladelser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="700d9-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="700d9-112">Føj enheder til Enhedsstyring ved at følge proceduren for onboarding af enheder.</span><span class="sxs-lookup"><span data-stu-id="700d9-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="700d9-113">Hvis du mangler indstillingen Tilføjelse af enhed (forhåndvisning) under M365 Compliance  **Settings**, skal du bekræfte, at du har den korrekte licens og de tilladelser, der henvises til ovenfor.</span><span class="sxs-lookup"><span data-stu-id="700d9-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="700d9-114">Du kan få mere at vide i [Tilføjelse af enheder](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="700d9-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="700d9-115">Opret DLP-politikker for at beskytte dine følsomme elementer.</span><span class="sxs-lookup"><span data-stu-id="700d9-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="700d9-116">Du kan få mere at vide i [Scenarier med Slutpunkt DLP-politik](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="700d9-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="700d9-117">Du kan finde flere oplysninger om Microsoft Endpoint DLP i [Få mere at vide om forebyggelse af datatab for Microsoft 365 Endpoint (prøveversion)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="700d9-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="700d9-118">**Vigtige trin til indsamling af data, hvis der er behov for støtte:**</span><span class="sxs-lookup"><span data-stu-id="700d9-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="700d9-119">Hent prøveversionen af MDATP-klientanalyse fra [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="700d9-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="700d9-120">Kør værktøjet som administrator fra cmd-vinduet:</span><span class="sxs-lookup"><span data-stu-id="700d9-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="700d9-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="700d9-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="700d9-122">Når du bliver bedt om at "angive antal minutter til indsamling af spor: ", skal du angive det antal minutter, der kræves for at køre scenariet</span><span class="sxs-lookup"><span data-stu-id="700d9-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="700d9-123">Kør scenariet</span><span class="sxs-lookup"><span data-stu-id="700d9-123">Run the scenario</span></span>

<span data-ttu-id="700d9-124">Indsaml det zipfil-output, der skal gives til supportmedarbejderen.</span><span class="sxs-lookup"><span data-stu-id="700d9-124">Collect the Zip file output to be given to the Support agent.</span></span>
