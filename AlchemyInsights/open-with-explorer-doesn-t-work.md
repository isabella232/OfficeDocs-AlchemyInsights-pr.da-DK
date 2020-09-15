---
title: Åbn med Stifinder virker ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694450"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="00a27-102">Åbn med Stifinder fungerer ikke</span><span class="sxs-lookup"><span data-stu-id="00a27-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="00a27-103">Hvis **Åbn med Stifinder** eller **Vis i Stifinder** ikke fungerer, skal du sikre dig, at WebClient-tjenesten er indstillet til at **køre** ved at følge nedenstående trin.</span><span class="sxs-lookup"><span data-stu-id="00a27-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="00a27-104">For eksempel kan det tage lang tid at åbne et SharePoint-eller OneDrive-bibliotek, når tjenesten ikke kører.</span><span class="sxs-lookup"><span data-stu-id="00a27-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="00a27-105">Skriv Kør i feltet Windows Search, Vælg appen Kør skrivebord, skriv Services. msc, og vælg derefter **Enter**.</span><span class="sxs-lookup"><span data-stu-id="00a27-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="00a27-106">Rul ned til tjenesten Webklient, og Markér kolonnen **status** .</span><span class="sxs-lookup"><span data-stu-id="00a27-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="00a27-107">Hvis WebClient-Tjenestestatus ikke **kører**, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="00a27-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="00a27-108">Aktivér tjenesten, hvis det er nødvendigt, ved at vælge enten **manuelt** eller **automatisk** i feltet **starttype** .</span><span class="sxs-lookup"><span data-stu-id="00a27-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="00a27-109">Hvis du vil foretage fejlfinding af problemer, der åbnes i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="00a27-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="00a27-110">Udforsk Synkroniser som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="00a27-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

