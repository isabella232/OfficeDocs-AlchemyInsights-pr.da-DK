---
title: Foretage fejlfinding af problemer ved hjælp af Åbn med Stifinder
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 5be8a8f9f67939c7e2671855da259818269d9299
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29464593"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="35c40-102">Løse problemer med Åbn med Stifinder</span><span class="sxs-lookup"><span data-stu-id="35c40-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="35c40-103">Løse almindelige problemer med at åbne et dokumentbibliotek i SharePoint- eller OneDrive ved hjælp af kommandoen **Åbn med Stifinder** :</span><span class="sxs-lookup"><span data-stu-id="35c40-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="35c40-p101">Brug Internet Explorer 10 eller Internet Explorer 11. **Åbn med Stifinder** ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Åbn med Stifinder** er deaktiveret i alle browsere, med undtagelse af Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="35c40-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="35c40-p102">**Åbn med Stifinder** er ikke tilgængelig i den moderne oplevelse for SharePoint-biblioteker. I stedet for at bruge **Vis i Stifinder** . Vælg **visningsindstillinger** \> **Vis i Stifinder**. Vis i Stifinder er ikke kompatibel med Microsoft Edge, Google Chrome, Firefox og andre. **Vis i Stifinder** i kun tilgængelig i Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="35c40-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="35c40-p103">Kontroller, at tjenesten WebClient kører. I Windows søgefeltet, Skriv Kør, Vælg Kør stationære programmet, skriv services.msc, og tryk derefter på Enter. Rul ned til tjenesten WebClient, og Sørg for, at kolonnen **Status** viser "Kørsel". Hvis det ikke er tilfældet, skal du dobbeltklikke på tjenesten, klik på **Start**og klik derefter på **OK**. (Du skal muligvis først aktivere tjenesten ved at vælge enten **Manuel** eller **automatisk** i **boksen** ).</span><span class="sxs-lookup"><span data-stu-id="35c40-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="35c40-p104">Åbne et bibliotek i Stifinder er praktisk, hvis du vil kopiere eller flytte flere filer og mapper, når, men hvis du vil arbejde regelmæssigt i biblioteket, anbefaler vi synkroniserer den. Hvis du vil foretage fejlfinding af problemer, der er åbne i Filoversigt, se [åbne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Du kan finde oplysninger om konfiguration af synkronisering, [Synkroniser SharePoint-filer med den nye OneDrive sync-klient](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="35c40-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="35c40-120">Se artiklen [Sådan bruges kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for at få yderligere oplysninger.</span><span class="sxs-lookup"><span data-stu-id="35c40-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

