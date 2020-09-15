---
title: Fejlfinding af problemer ved hjælp af Åbn med Stifinder
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659052"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="22393-102">Løs problemer med Åbn med Stifinder</span><span class="sxs-lookup"><span data-stu-id="22393-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="22393-103">Løse almindelige problemer med at åbne et dokumentbibliotek i SharePoint eller OneDrive ved hjælp af kommandoen **Åbn med Stifinder** :</span><span class="sxs-lookup"><span data-stu-id="22393-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="22393-104">Brug Internet Explorer 10 eller Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="22393-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="22393-105">**Åbn med Stifinder** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="22393-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="22393-106">**Åbn med Stifinder** er deaktiveret i alle browsere undtagen Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="22393-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="22393-107">**Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint-biblioteker.</span><span class="sxs-lookup"><span data-stu-id="22393-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="22393-108">Brug **visningen i Stifinder i** stedet.</span><span class="sxs-lookup"><span data-stu-id="22393-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="22393-109">Vælg visningen **Indstillinger for visning** \> **i Stifinder**.</span><span class="sxs-lookup"><span data-stu-id="22393-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="22393-110">Visning i Stifinder er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="22393-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="22393-111">**Vis i Stifinder** i kun tilgængelig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="22393-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="22393-112">Sørg for, at WebClient-tjenesten kører.</span><span class="sxs-lookup"><span data-stu-id="22393-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="22393-113">Skriv Kør i feltet Windows Search, Vælg appen Kør skrivebord, skriv Services. msc, og tryk derefter på ENTER.</span><span class="sxs-lookup"><span data-stu-id="22393-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="22393-114">Rul ned til WebClient-tjenesten, og sørg for, at **status** kolonnen viser "kører".</span><span class="sxs-lookup"><span data-stu-id="22393-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="22393-115">Hvis det ikke er det, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="22393-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="22393-116">(Du skal muligvis først aktivere tjenesten ved enten at vælge **Manuel** eller **automatisk** i feltet **starttype** .)</span><span class="sxs-lookup"><span data-stu-id="22393-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="22393-117">Det anbefales at åbne et bibliotek i Stifinder, hvis du har brug for at kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbejde regelmæssigt i biblioteket, anbefaler vi at synkronisere det.</span><span class="sxs-lookup"><span data-stu-id="22393-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="22393-118">Hvis du vil foretage fejlfinding af problemer, der åbnes i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="22393-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="22393-119">Du kan finde oplysninger om, hvordan du konfigurerer synkronisering, under [synkronisere SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="22393-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="22393-120">Læs artiklen [Sådan bruger du kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online for at](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="22393-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

