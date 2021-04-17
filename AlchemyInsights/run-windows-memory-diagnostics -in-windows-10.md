---
title: Kør Windows Hukommelsesdiagnosticering i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826661"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="dbe33-102">Kør Windows Hukommelsesdiagnosticering i Windows 10</span><span class="sxs-lookup"><span data-stu-id="dbe33-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="dbe33-103">Hvis Windows og apps på din pc går ned, fryser eller fungerer ustabilt, kan der være problemer med pc'ens hukommelse (RAM).</span><span class="sxs-lookup"><span data-stu-id="dbe33-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="dbe33-104">Du kan køre Windows Hukommelsesdiagnosticering for at kontrollere, om der er problemer med pc'ens RAM.</span><span class="sxs-lookup"><span data-stu-id="dbe33-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="dbe33-105">Skriv hukommelsesdiagnosticering i **søgefeltet på proceslinjen,** og vælg derefter **Windows Hukommelsesdiagnosticering.**</span><span class="sxs-lookup"><span data-stu-id="dbe33-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="dbe33-106">Pc'en skal genstartes for at køre diagnosticeringen.</span><span class="sxs-lookup"><span data-stu-id="dbe33-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="dbe33-107">Du har mulighed for at genstarte med det samme (gem dit arbejde, og luk åbne dokumenter og mails først), eller planlæg diagnosticeringen til at køre automatisk, næste gang pc'en genstarter:</span><span class="sxs-lookup"><span data-stu-id="dbe33-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Hukommelsesdiagnosticering](media/windows-memory-diagnostic.png)

<span data-ttu-id="dbe33-109">Når pc'en genstarter, **kører Windows Hukommelsesdiagnosticering** automatisk.</span><span class="sxs-lookup"><span data-stu-id="dbe33-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="dbe33-110">Status og status vises i diagnosticeringsværktøjet, og du kan annullere diagnosticeringen ved at trykke på **Esc** på tastaturet.</span><span class="sxs-lookup"><span data-stu-id="dbe33-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="dbe33-111">Når diagnosticeringen er fuldført, starter Windows normalt.</span><span class="sxs-lookup"><span data-stu-id="dbe33-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="dbe33-112">Straks efter genstart, når skrivebordet vises, vises der  en meddelelse (ud for ikonet Handlingscenter på proceslinjen) for at angive, om der blev fundet hukommelsesfejl.</span><span class="sxs-lookup"><span data-stu-id="dbe33-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="dbe33-113">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="dbe33-113">For example:</span></span>

<span data-ttu-id="dbe33-114">Her er ikonet Handlingscenter:</span><span class="sxs-lookup"><span data-stu-id="dbe33-114">Here's the Action Center icon:</span></span> ![Ikonet Handlingscenter](media/action-center-icon.png) 

<span data-ttu-id="dbe33-116">Og en eksempelmeddelelse:</span><span class="sxs-lookup"><span data-stu-id="dbe33-116">And a sample notification:</span></span> ![Ingen hukommelsesfejl](media/no-memory-errors.png)

<span data-ttu-id="dbe33-118">Hvis du ikke når at  se meddelelsen, kan du  vælge ikonet handlingscenter på proceslinjen for at få vist Handlingscenter og få vist en liste over meddelelser, der kan rulles i.</span><span class="sxs-lookup"><span data-stu-id="dbe33-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="dbe33-119">Hvis du vil gennemse detaljerede oplysninger, **skal** du skrive begivenhed i søgefeltet på proceslinjen og derefter vælge **Log på**.</span><span class="sxs-lookup"><span data-stu-id="dbe33-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="dbe33-120">I **ruden til** venstre for Logbog skal du gå til **Windows-logge > System.**</span><span class="sxs-lookup"><span data-stu-id="dbe33-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="dbe33-121">I højre rude skal du rulle ned på  listen, mens du kigger på kolonnen Kilde, indtil du ser hændelser med kildeværdien **MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="dbe33-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="dbe33-122">Fremhæv hver enkelt begivenhed, og få vist resultatoplysningerne i feltet under **fanen** Generelt under listen.</span><span class="sxs-lookup"><span data-stu-id="dbe33-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
