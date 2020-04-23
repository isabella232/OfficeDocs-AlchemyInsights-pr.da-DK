---
title: Fejlfinding i forbindelse med problemer ved hjælp af Åbn med Stifinder
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759686"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="90943-102">Løs problemer med Åbn med Stifinder</span><span class="sxs-lookup"><span data-stu-id="90943-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="90943-103">Løs almindelige problemer med at åbne et dokumentbibliotek i SharePoint eller OneDrive ved hjælp af kommandoen **Åbn med Stifinder:**</span><span class="sxs-lookup"><span data-stu-id="90943-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="90943-104">Brug Internet Explorer 10 eller Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="90943-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="90943-105">**Åbn med Explorer** er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre.</span><span class="sxs-lookup"><span data-stu-id="90943-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="90943-106">**Åbn med Stifinder** er deaktiveret i alle browsere undtagen Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="90943-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="90943-107">**Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint-biblioteker.</span><span class="sxs-lookup"><span data-stu-id="90943-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="90943-108">Brug i stedet **Vis i Stifinder.**</span><span class="sxs-lookup"><span data-stu-id="90943-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="90943-109">Vælg **Vis indstillinger** \> **Vis i Stifinder**.</span><span class="sxs-lookup"><span data-stu-id="90943-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="90943-110">Visningen i Stifinder er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox m.fl.</span><span class="sxs-lookup"><span data-stu-id="90943-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="90943-111">**Få vist i Stifinder** i Kun tilgængelig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="90943-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="90943-112">Kontroller, at webclient-tjenesten kører.</span><span class="sxs-lookup"><span data-stu-id="90943-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="90943-113">Skriv kør i søgefeltet i Windows, vælg appen Kør skrivebord, skriv services.msc, og tryk derefter på Enter.</span><span class="sxs-lookup"><span data-stu-id="90943-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="90943-114">Rul ned til tjenesten WebClient, og sørg for, at kolonnen **Status** viser "Kørsel".</span><span class="sxs-lookup"><span data-stu-id="90943-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="90943-115">Hvis det ikke er tilfældet, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**.</span><span class="sxs-lookup"><span data-stu-id="90943-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="90943-116">(Du skal muligvis først aktivere tjenesten ved at vælge enten **Manuel** eller **Automatisk** i feltet **Starttype).**</span><span class="sxs-lookup"><span data-stu-id="90943-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="90943-117">Det er praktisk at åbne et bibliotek i Stifinder, hvis du har brug for at kopiere eller flytte flere filer og mapper én gang, men hvis du vil arbejde regelmæssigt i biblioteket, anbefaler vi, at du synkroniserer det.</span><span class="sxs-lookup"><span data-stu-id="90943-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="90943-118">Hvis du vil foretage fejlfinding af problemer med at åbne i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="90943-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="90943-119">Du kan finde oplysninger om konfiguration af synkronisering under [Synkronisere SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="90943-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="90943-120">Se artiklen [Sådan bruges kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for at få flere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="90943-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

