---
title: Diagram viser forskellige antal poster i gitter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439003"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="9c0b1-102">Diagram viser forskellige antal poster i gitter</span><span class="sxs-lookup"><span data-stu-id="9c0b1-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="9c0b1-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="9c0b1-103">**Symptom**</span></span>

<span data-ttu-id="9c0b1-104">For diagram på dashboard side, når du klikker på diagrammet "..." og klik på "Vis poster", skal du navigere til gittersiden for at se alle posterne. Nogle gange ændres antallet af poster.</span><span class="sxs-lookup"><span data-stu-id="9c0b1-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="9c0b1-105">**Forårsage**</span><span class="sxs-lookup"><span data-stu-id="9c0b1-105">**Cause**</span></span>

<span data-ttu-id="9c0b1-106">Dette skyldes forskellen mellem visningerne mellem diagrammet på den oprindelige dashboardside og diagrammet på gitterets startside.</span><span class="sxs-lookup"><span data-stu-id="9c0b1-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="9c0b1-107">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="9c0b1-107">**Solution**</span></span>

1. <span data-ttu-id="9c0b1-108">Kontroller visningen fra den oprindelige side og visningen i gitteret for at se, om de er forskellige.</span><span class="sxs-lookup"><span data-stu-id="9c0b1-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="9c0b1-109">Rediger visningen i gitteret, så den svarer til visningen på den oprindelige side.</span><span class="sxs-lookup"><span data-stu-id="9c0b1-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="9c0b1-110">Hvis den korrekte visning ikke kan findes, betyder det normalt, at visningen ikke er aktiveret i appdesigner.</span><span class="sxs-lookup"><span data-stu-id="9c0b1-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="9c0b1-111">Gå til appdesigner for den specifikke app, vælg objektet og dets visninger, markér den visning, du vil aktivere, gemme, udgive og lukke.</span><span class="sxs-lookup"><span data-stu-id="9c0b1-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="9c0b1-112">Opdater siden.</span><span class="sxs-lookup"><span data-stu-id="9c0b1-112">Refresh the page.</span></span>