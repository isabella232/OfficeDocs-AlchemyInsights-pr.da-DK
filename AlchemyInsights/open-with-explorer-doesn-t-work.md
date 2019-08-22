---
title: Åbn med Stifinder virker ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538460"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="f2593-102">Åbn med Stifinder fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="f2593-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="f2593-103">Kontroller, at tjenesten WebClient er indstillet til at **køre** ved at benytte følgende fremgangsmåde, hvis **Åbn med Stifinder** eller **visning i File Explorer** ikke virker.</span><span class="sxs-lookup"><span data-stu-id="f2593-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="f2593-104">For eksempel kan det tage lang tid at åbne et SharePoint- eller OneDrive-bibliotek, når tjenesten ikke kører.</span><span class="sxs-lookup"><span data-stu-id="f2593-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="f2593-105">I feltet Windows Søg type Kør, Vælg Kør desktop app, skriv services.msc, og vælg derefter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="f2593-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="f2593-106">Rul ned til tjenesten WebClient, og se i kolonnen **Status** .</span><span class="sxs-lookup"><span data-stu-id="f2593-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="f2593-107">Hvis status for tjenesten WebClient ikke er **kører**, dobbeltklik på tjenesten, klikke på **Start**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="f2593-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="f2593-108">Aktivere tjenesten, hvis det er nødvendigt, ved at vælge enten **Manuel** eller **automatisk** i **boksen** .</span><span class="sxs-lookup"><span data-stu-id="f2593-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="f2593-109">Hvis du vil foretage fejlfinding af problemer, der er åbne i Filoversigt, se [åbne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="f2593-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="f2593-110">Udforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive sync-klient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="f2593-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

