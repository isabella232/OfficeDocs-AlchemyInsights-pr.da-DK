---
title: Diagram viser et andet antal poster i gitter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793752"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="7ba08-102">Diagram viser et andet antal poster i gitter</span><span class="sxs-lookup"><span data-stu-id="7ba08-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="7ba08-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="7ba08-103">**Symptom**</span></span>

<span data-ttu-id="7ba08-104">For diagram på dashboardsiden, når du klikker på diagram "..." og klik på "Vis poster", skal du gå til gitter side for at få vist alle posterne. Nogle gange ændres antallet af poster.</span><span class="sxs-lookup"><span data-stu-id="7ba08-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="7ba08-105">**Kræve**</span><span class="sxs-lookup"><span data-stu-id="7ba08-105">**Cause**</span></span>

<span data-ttu-id="7ba08-106">Dette skyldes forskellen mellem visningen af diagrammet på den oprindelige dashboardside og diagrammet på gitter startsiden.</span><span class="sxs-lookup"><span data-stu-id="7ba08-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="7ba08-107">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="7ba08-107">**Solution**</span></span>

1. <span data-ttu-id="7ba08-108">Markér visningen på den oprindelige side og visningen i gitteret for at se, om de er forskellige.</span><span class="sxs-lookup"><span data-stu-id="7ba08-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="7ba08-109">Du kan ændre visningen i gitteret, så det svarer til visningen på den oprindelige side.</span><span class="sxs-lookup"><span data-stu-id="7ba08-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="7ba08-110">Hvis den korrekte visning ikke kan findes, betyder det normalt, at visningen ikke er aktiveret i app designer.</span><span class="sxs-lookup"><span data-stu-id="7ba08-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="7ba08-111">Gå til App designer for den bestemte app, Vælg objektet og dens visninger, Markér den visning, du vil aktivere, gemme, publicere og lukke.</span><span class="sxs-lookup"><span data-stu-id="7ba08-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="7ba08-112">Opdater siden.</span><span class="sxs-lookup"><span data-stu-id="7ba08-112">Refresh the page.</span></span>