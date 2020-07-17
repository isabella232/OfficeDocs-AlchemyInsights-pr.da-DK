---
title: Problemet med udskriftsspooler er løst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088304"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="dd504-102">Problemet med udskriftsspooler er løst</span><span class="sxs-lookup"><span data-stu-id="dd504-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="dd504-103">Hvis enheden er blevet opdateret med Windows 10 **OS Build 19041.329**, har du muligvis observeret et problem, hvor visse printere ikke udskrives.</span><span class="sxs-lookup"><span data-stu-id="dd504-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="dd504-104">Udskriftsspooleren kan kaste en fejl eller lukke uventet, når du forsøger at udskrive, og der kommer ingen udgang fra den berørte printer.</span><span class="sxs-lookup"><span data-stu-id="dd504-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="dd504-105">Dette problem er løst i OS Build **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="dd504-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="dd504-106">**Igangværende undersøgelse**</span><span class="sxs-lookup"><span data-stu-id="dd504-106">**Ongoing investigation**</span></span>

<span data-ttu-id="dd504-107">LSASS-filen (Local Security Authority Subsystem Service)\*\* (Isass.exe\*\*) kan mislykkes på nogle enheder med fejlmeddelelsen "En kritisk systemproces, C:\WINDOWS\system32\Isass.exe mislykkedes med statuskoden c0000008.</span><span class="sxs-lookup"><span data-stu-id="dd504-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="dd504-108">Maskinen skal nu genstartes".</span><span class="sxs-lookup"><span data-stu-id="dd504-108">The machine must now be restarted".</span></span>  <span data-ttu-id="dd504-109">**Microsoft arbejder på en løsning og leverer en opdatering i en kommende version.**</span><span class="sxs-lookup"><span data-stu-id="dd504-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="dd504-110">Du kan finde flere oplysninger i kendte problemer i [Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="dd504-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>