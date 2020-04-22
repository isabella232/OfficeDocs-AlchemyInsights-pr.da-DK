---
title: Åbn med Stifinder virker ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713028"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="e94c2-102">Åbn med Stifinder fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="e94c2-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="e94c2-103">Hvis **Åbn med Stifinder** eller **Vis i Stifinder** ikke virker, skal du sørge for, at webclient-tjenesten er indstillet til **Kørende** ved at følge nedenstående trin.</span><span class="sxs-lookup"><span data-stu-id="e94c2-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="e94c2-104">det kan for eksempel tage lang tid at åbne et SharePoint- eller OneDrive-bibliotek, når tjenesten ikke kører.</span><span class="sxs-lookup"><span data-stu-id="e94c2-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="e94c2-105">Skriv kør i søgefeltet i Windows, vælg appen Kør skrivebord, skriv services.msc, og vælg derefter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e94c2-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="e94c2-106">Rul ned til tjenesten WebClient, og kontroller kolonnen **Status.**</span><span class="sxs-lookup"><span data-stu-id="e94c2-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="e94c2-107">Hvis webclient-tjenestestatus ikke **kører**, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="e94c2-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e94c2-108">Aktivér tjenesten, hvis det er nødvendigt, ved at vælge enten **Manuel** eller **Automatisk** i feltet **Starttype.**</span><span class="sxs-lookup"><span data-stu-id="e94c2-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e94c2-109">Hvis du vil foretage fejlfinding af problemer med at åbne i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="e94c2-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e94c2-110">Udforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e94c2-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

