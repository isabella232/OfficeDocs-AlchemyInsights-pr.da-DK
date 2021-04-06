---
title: Service diagnostics tool for Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595515"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="9e185-102">Service diagnostics tool for Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="9e185-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="9e185-103">WVD (Windows Virtual Desktop) tilbyder et diagnosticeringsværktøj, der gør det muligt for administratorer at identificere fejl via en enkelt grænseflade.</span><span class="sxs-lookup"><span data-stu-id="9e185-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="9e185-104">Dette værktøj logføres diagnosticeringsrelaterede oplysninger, når WVD bruges af en person, der er tildelt en WVD-rolle.</span><span class="sxs-lookup"><span data-stu-id="9e185-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="9e185-105">Hver log indeholder oplysninger om den WVD-rolle, der er involveret i aktiviteten, de fejlmeddelelser, der vises under sessionen, og oplysninger om lejeren og brugeren.</span><span class="sxs-lookup"><span data-stu-id="9e185-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="9e185-106">Azure Log Analytics kan konfigureres til at registrere den aktivitetslog, der er oprettet af diagnosticeringsværktøjet, ved at følge disse trin:</span><span class="sxs-lookup"><span data-stu-id="9e185-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="9e185-107">Opret et loganalysearbejdsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="9e185-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="9e185-108">[Forbind Windows-computere til Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="9e185-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="9e185-109">Hent arbejdsområde-id'et og den primære nøgle for arbejdsområdet.</span><span class="sxs-lookup"><span data-stu-id="9e185-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="9e185-110">Konfigurationsguiden skal bruge disse oplysninger for at konfigurere agenten korrekt og for at sikre, at den kan kommunikere med Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="9e185-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="9e185-111">[Skubbe diagnosticeringsdata til arbejdsområdet.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="9e185-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="9e185-112">Du kan skubbe diagnostiske data fra din WVD-lejer til Log Analytics for dit arbejdsområde.</span><span class="sxs-lookup"><span data-stu-id="9e185-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="9e185-113">[Identificer](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) og diagnosticer problemer, der er interne eller eksterne i forhold til WVD.</span><span class="sxs-lookup"><span data-stu-id="9e185-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="9e185-114">Hvis du vil have mere at vide om konfiguration af værktøjet til tjenestediagnosticering til WVD, skal du se Brug loganalyse til diagnosticeringsfunktionen.</span><span class="sxs-lookup"><span data-stu-id="9e185-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>