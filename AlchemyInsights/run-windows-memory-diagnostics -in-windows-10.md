---
title: Kør Windows Hukommelsesdiagnosticering i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720784"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="e3394-102">Kør Windows Hukommelsesdiagnosticering i Windows 10</span><span class="sxs-lookup"><span data-stu-id="e3394-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="e3394-103">Hvis Windows og apps på din PC går ned, fryser eller reagerer på en ustabil måde, kan der være et problem med pc'ens hukommelse (RAM).</span><span class="sxs-lookup"><span data-stu-id="e3394-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="e3394-104">Du kan køre Windows Hukommelsesdiagnosticering for at kontrollere, om der er problemer med pc'ens RAM.</span><span class="sxs-lookup"><span data-stu-id="e3394-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="e3394-105">Skriv **hukommelsesdiagnosticering**i søgefeltet på proceslinjen, og vælg derefter **Windows Hukommelsesdiagnosticering**.</span><span class="sxs-lookup"><span data-stu-id="e3394-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="e3394-106">Hvis du vil køre diagnosticeringen, skal du genstarte computeren.</span><span class="sxs-lookup"><span data-stu-id="e3394-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="e3394-107">Du har mulighed for at genstarte med det samme (Gem dit arbejde, og Luk åbne dokumenter og mails først), eller Planlæg diagnosticeringen til at køre automatisk, næste gang PC genstartes:</span><span class="sxs-lookup"><span data-stu-id="e3394-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows Hukommelsesdiagnosticering](media/windows-memory-diagnostic.png)

<span data-ttu-id="e3394-109">Når pc'en genstartes, kører **værktøjet Windows Hukommelsesdiagnosticering** automatisk.</span><span class="sxs-lookup"><span data-stu-id="e3394-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="e3394-110">Status og status vises, når diagnosticeringen kører, og du har mulighed for at annullere diagnosticeringen ved at trykke på **ESC** -tasten på tastaturet.</span><span class="sxs-lookup"><span data-stu-id="e3394-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="e3394-111">Når diagnosticeringen er fuldført, vil Windows starte normalt.</span><span class="sxs-lookup"><span data-stu-id="e3394-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="e3394-112">Når skrivebordet vises umiddelbart efter genstart, vises der en meddelelse (ved siden af **handlings Center** -ikonet på proceslinjen) for at angive, om der er fundet hukommelsesfejl.</span><span class="sxs-lookup"><span data-stu-id="e3394-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="e3394-113">Det kan f.eks. være:</span><span class="sxs-lookup"><span data-stu-id="e3394-113">For example:</span></span>

<span data-ttu-id="e3394-114">Her er ikonet for løsnings Centeret:</span><span class="sxs-lookup"><span data-stu-id="e3394-114">Here's the Action Center icon:</span></span> ![Handlingscenter-ikon](media/action-center-icon.png) 

<span data-ttu-id="e3394-116">Og et eksempel på en meddelelse:</span><span class="sxs-lookup"><span data-stu-id="e3394-116">And a sample notification:</span></span> ![Ingen hukommelsesfejl](media/no-memory-errors.png)

<span data-ttu-id="e3394-118">Hvis du ikke har mistet beskeden, kan du vælge ikonet for **handlingscenter** på proceslinjen for at få vist **Løsningscenter** og få vist en liste over meddelelser, der kan rulles i.</span><span class="sxs-lookup"><span data-stu-id="e3394-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="e3394-119">Hvis du vil gennemgå detaljerede oplysninger, skal du skrive **begivenhed** i søgefeltet på proceslinjen og derefter vælge **Logbog**.</span><span class="sxs-lookup"><span data-stu-id="e3394-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="e3394-120">I **logbogens**venstre rude skal du gå til **Windows Logs > system**.</span><span class="sxs-lookup"><span data-stu-id="e3394-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="e3394-121">I højre rude skal du scanne ned på listen, mens du kigger på **kilde** kolonnen, indtil du ser begivenheder med kildeværdien **MemoryDiagnostics-resultater**.</span><span class="sxs-lookup"><span data-stu-id="e3394-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="e3394-122">Fremhæv hver enkelt begivenhed, og se resultat oplysningerne i feltet under fanen **Generelt** under listen.</span><span class="sxs-lookup"><span data-stu-id="e3394-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
