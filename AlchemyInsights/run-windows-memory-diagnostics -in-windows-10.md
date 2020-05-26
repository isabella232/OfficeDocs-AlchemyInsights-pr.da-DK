---
title: Køre Windows Hukommelsesdiagnosticering i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357378"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="c8cca-102">Køre Windows Hukommelsesdiagnosticering i Windows 10</span><span class="sxs-lookup"><span data-stu-id="c8cca-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="c8cca-103">Hvis Windows og apps på din pc går ned, fryser eller handler ustabilt, kan du have et problem med pc'ens hukommelse (RAM).</span><span class="sxs-lookup"><span data-stu-id="c8cca-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="c8cca-104">Du kan køre Windows Hukommelsesdiagnosticering for at kontrollere, om der er problemer med pc'ens RAM.</span><span class="sxs-lookup"><span data-stu-id="c8cca-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="c8cca-105">Skriv **hukommelsesdiagnosticering**i søgefeltet på proceslinjen, og vælg derefter **Windows Hukommelsesdiagnosticering**.</span><span class="sxs-lookup"><span data-stu-id="c8cca-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="c8cca-106">Hvis du vil køre diagnosticeringen, skal pc'en genstartes.</span><span class="sxs-lookup"><span data-stu-id="c8cca-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="c8cca-107">Du har mulighed for at genstarte med det samme (gem dit arbejde og luk åbne dokumenter og e-mails først), eller planlæg, at diagnosticeringen skal køre automatisk, næste gang pc'en genstarter:</span><span class="sxs-lookup"><span data-stu-id="c8cca-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnosticering af Windows-hukommelse](media/windows-memory-diagnostic.png)

<span data-ttu-id="c8cca-109">Når pc'en genstartes, kører **Windows Hukommelsesdiagnosticering** automatisk.</span><span class="sxs-lookup"><span data-stu-id="c8cca-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="c8cca-110">Status og status vises, mens diagnosticeringen kører, og du har mulighed for at annullere diagnosticeringen ved at trykke på **ESC-tasten** på tastaturet.</span><span class="sxs-lookup"><span data-stu-id="c8cca-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="c8cca-111">Når diagnosticeringen er fuldført, starter Windows normalt.</span><span class="sxs-lookup"><span data-stu-id="c8cca-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="c8cca-112">Umiddelbart efter genstartvises der en meddelelse (ud for ikonet **Løsningscenter** på proceslinjen) umiddelbart efter genstarten for at angive, om der er fundet hukommelsesfejl.</span><span class="sxs-lookup"><span data-stu-id="c8cca-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="c8cca-113">Det kan f.eks. være:</span><span class="sxs-lookup"><span data-stu-id="c8cca-113">For example:</span></span>

<span data-ttu-id="c8cca-114">Her er ikonet Løsningscenter:</span><span class="sxs-lookup"><span data-stu-id="c8cca-114">Here's the Action Center icon:</span></span> ![Ikon for Handlingscenter](media/action-center-icon.png) 

<span data-ttu-id="c8cca-116">Og en prøve anmeldelse:</span><span class="sxs-lookup"><span data-stu-id="c8cca-116">And a sample notification:</span></span> ![Ingen hukommelsesfejl](media/no-memory-errors.png)

<span data-ttu-id="c8cca-118">Hvis du ikke har modtaget meddelelsen, kan du vælge ikonet **Løsningscenter** på proceslinjen for at få vist **Løsningscenter** og se en liste over meddelelser, der kan rulles igennem.</span><span class="sxs-lookup"><span data-stu-id="c8cca-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="c8cca-119">Hvis du vil gennemse detaljerede oplysninger, skal du skrive **hændelse** i søgefeltet på proceslinjen og derefter vælge **Logbog**.</span><span class="sxs-lookup"><span data-stu-id="c8cca-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="c8cca-120">Gå til **Windows Logs > System**i **logbogs**venstre rude .</span><span class="sxs-lookup"><span data-stu-id="c8cca-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="c8cca-121">Skan ned på listen i højre rude, mens du ser på kolonnen **Kilde,** indtil du ser hændelser med Kildeværdien **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="c8cca-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="c8cca-122">Fremhæv hver af disse hændelser, og se resultatoplysningerne i feltet under fanen **Generelt** under listen.</span><span class="sxs-lookup"><span data-stu-id="c8cca-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
