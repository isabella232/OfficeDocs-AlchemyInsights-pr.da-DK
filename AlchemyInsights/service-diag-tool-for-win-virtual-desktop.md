---
title: Værktøjet tjeneste diagnosticering til Windows virtuelt skrivebord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677649"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="b7994-102">Værktøjet tjeneste diagnosticering til Windows virtuelt skrivebord</span><span class="sxs-lookup"><span data-stu-id="b7994-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="b7994-103">Windows virtuelt skrivebord (WVD) tilbyder et diagnosticeringsværktøj, der gør det muligt for administratorer at identificere fejl via en enkelt grænseflade.</span><span class="sxs-lookup"><span data-stu-id="b7994-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="b7994-104">Dette værktøj registrerer diagnosticerings relaterede oplysninger, når WVD bruges af en person, der har fået tildelt en WVD-rolle.</span><span class="sxs-lookup"><span data-stu-id="b7994-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="b7994-105">Hver log indeholder oplysninger om den WVD-rolle, der er involveret i aktiviteten, de fejlmeddelelser, der vises under sessionen, og oplysningerne om lejeren og brugeren.</span><span class="sxs-lookup"><span data-stu-id="b7994-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="b7994-106">Azure log Analytics kan konfigureres til at registrere aktivitetslogfilen, der er oprettet af værktøjet diagnosticering.</span><span class="sxs-lookup"><span data-stu-id="b7994-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="b7994-107">Sådan gør du:</span><span class="sxs-lookup"><span data-stu-id="b7994-107">Here's how:</span></span>

1. <span data-ttu-id="b7994-108">Oprette et log Analytics-arbejdsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="b7994-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="b7994-109">[Oprette forbindelse mellem Windows-computere og Azure-skærm](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="b7994-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="b7994-110">Hent arbejdsområde-id'et og den primære nøgle i dit arbejdsområde.</span><span class="sxs-lookup"><span data-stu-id="b7994-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="b7994-111">Konfigurationsguiden skal have disse oplysninger for at konfigurere agenten korrekt og sikre, at den kan kommunikere med Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="b7994-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="b7994-112">[Overfør diagnosticeringsdata til arbejdsområdet](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="b7994-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="b7994-113">Du kan skubbe diagnosticeringsdata fra din WVD-lejer til en logfils analyse for dit arbejdsområde.</span><span class="sxs-lookup"><span data-stu-id="b7994-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="b7994-114">[Identificer og Diagnosticer problemer](https://go.microsoft.com/fwlink/?linkid=2128338) , der er interne eller eksterne i forhold til WVD.</span><span class="sxs-lookup"><span data-stu-id="b7994-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="b7994-115">Hvis du vil have mere at vide om konfiguration af værktøjet til tjeneste diagnosticering for WVD, skal du se [brug af log analyse til diagnosticerings funktionen](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="b7994-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
