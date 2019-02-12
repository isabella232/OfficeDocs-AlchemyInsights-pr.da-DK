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
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906798"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="a1cd5-102">Åbn med Stifinder fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="a1cd5-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="a1cd5-p101">Kontroller, at tjenesten WebClient er indstillet til at **køre** ved at benytte følgende fremgangsmåde, hvis **Åbn med Stifinder** eller **visning i File Explorer** ikke virker. For eksempel kan det tage lang tid at åbne et SharePoint- eller OneDrive-bibliotek, når tjenesten ikke kører.</span><span class="sxs-lookup"><span data-stu-id="a1cd5-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="a1cd5-105">I feltet Windows Søg type Kør, Vælg Kør desktop app, skriv services.msc, og vælg derefter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a1cd5-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="a1cd5-p102">Rul ned til tjenesten WebClient, og se i kolonnen **Status** . Hvis status for tjenesten WebClient ikke er **kører**, dobbeltklik på tjenesten, klikke på **Start**og derefter klikke på **OK**. Aktivere tjenesten, hvis det er nødvendigt, ved at vælge enten **Manuel** eller **automatisk** i **boksen** .</span><span class="sxs-lookup"><span data-stu-id="a1cd5-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a1cd5-p103">Hvis du vil foretage fejlfinding af problemer, der er åbne i Filoversigt, se [åbne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Udforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive sync-klient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="a1cd5-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

