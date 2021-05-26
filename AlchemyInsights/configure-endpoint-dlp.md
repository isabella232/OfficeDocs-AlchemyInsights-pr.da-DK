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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657923"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="8768a-102">Konfigurer Slutpunkt DLP</span><span class="sxs-lookup"><span data-stu-id="8768a-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="8768a-103">Microsoft Slutpunkt DLP giver dig mulighed at udvide DLP-beskyttelse og overvågning til følsomme oplysninger på Windows 10-enheder.</span><span class="sxs-lookup"><span data-stu-id="8768a-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="8768a-104">Når enheder er integreret i enhedsstyring, kan du oprette DLP-politikker for at gennemtvinge beskyttende handlinger for elementer.</span><span class="sxs-lookup"><span data-stu-id="8768a-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="8768a-105">Aktivitetsoversigten kan bruges til at overvåge aktivitet for følsomme elementer.</span><span class="sxs-lookup"><span data-stu-id="8768a-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="8768a-106">Du kan få mere at vide under [Tilføjelse af enheder til enhedsstyring](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="8768a-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="8768a-107">Sådan kommer du i gang med Slutpunkt DLP:</span><span class="sxs-lookup"><span data-stu-id="8768a-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="8768a-108">Sørg for, at du har den rette SKU/abonnementslicens.</span><span class="sxs-lookup"><span data-stu-id="8768a-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="8768a-109">Du kan finde flere oplysninger i[Licenser til SKU/abonnementer](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="8768a-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="8768a-110">Kontrollér de tilladelser, der kræves for at aktivere enhedsstyring, få adgang til onboarding-siden eller aktivere/deaktivere overvågning af enheder.</span><span class="sxs-lookup"><span data-stu-id="8768a-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="8768a-111">Du kan finde flere oplysninger under [Tilladelser](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="8768a-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="8768a-112">Føj enheder til Enhedsstyring ved at følge proceduren for onboarding af enheder.</span><span class="sxs-lookup"><span data-stu-id="8768a-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="8768a-113">Du kan få mere at vide i [Tilføjelse af enheder](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="8768a-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="8768a-114">Opret DLP-politikker for at beskytte dine følsomme elementer.</span><span class="sxs-lookup"><span data-stu-id="8768a-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="8768a-115">Du kan få mere at vide i [Scenarier med Slutpunkt DLP-politik](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="8768a-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="8768a-116">Du kan finde flere oplysninger om Microsoft Endpoint DLP i [Få mere at vide om forebyggelse af datatab for Microsoft 365 Endpoint (prøveversion)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="8768a-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="8768a-117">**Vigtige trin til indsamling af data, hvis der er behov for støtte:**</span><span class="sxs-lookup"><span data-stu-id="8768a-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="8768a-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="8768a-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="8768a-119">Kør værktøjet som administrator fra cmd-vinduet:</span><span class="sxs-lookup"><span data-stu-id="8768a-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="8768a-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="8768a-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="8768a-121">Når du bliver bedt om det, angiv det antal minutter, der skal bruges til at indsamle **sporinger:**, angiv det antal minutter, der kræves for at køre scenariet.</span><span class="sxs-lookup"><span data-stu-id="8768a-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="8768a-122">Kør scenariet.</span><span class="sxs-lookup"><span data-stu-id="8768a-122">Run the scenario.</span></span>

<span data-ttu-id="8768a-123">Indsaml zip-filoutput for at give det til supportmedarbejderen.</span><span class="sxs-lookup"><span data-stu-id="8768a-123">Collect the Zip file output to give to the Support agent.</span></span>
