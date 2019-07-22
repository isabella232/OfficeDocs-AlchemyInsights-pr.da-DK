---
title: Foretag fejlfinding af "Åbn med Stifinder" i SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 13149d288336b487441c66521b32406e408911fd
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35803032"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="6a015-102">Foretag fejlfinding af "Åbn med Stifinder" i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6a015-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="6a015-103">Kommandoen Åbn med Stifinder åbner en lokal forekomst af Windows Stifinder, der viser mappestrukturen på den server, hvor SharePoint-webstedet er hostet.</span><span class="sxs-lookup"><span data-stu-id="6a015-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="6a015-104">Det anbefales dog, at du [synkroniserer SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, der giver mulighed for [Filer efter behov](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), fordi det giver lokal adgang til dine filer og den bedste ydeevne.</span><span class="sxs-lookup"><span data-stu-id="6a015-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="6a015-105">Hvis du vælger at bruge Stifinder-visningen i stedet for at bruge den nye OneDrive-synkroniseringsklient, skal du sikre dig, at du følger trinnene og de bedste fremgangsmåder i de følgende artikler:</span><span class="sxs-lookup"><span data-stu-id="6a015-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="6a015-106">Sådan bruger du kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6a015-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="6a015-107">Kopiér eller flyt biblioteksfiler ved hjælp af Åbn med Stifinder</span><span class="sxs-lookup"><span data-stu-id="6a015-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="6a015-108">Knappen **Åbn med Stifinder** vises ikke i den nye biblioteksoplevelse.</span><span class="sxs-lookup"><span data-stu-id="6a015-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="6a015-109">Vælg rullemenuen **Vis** øverst til højre (navnet på rullemenuen afhænger af, hvilken visning du i øjeblikket bruger), og vælg derefter **Vis i Stifinder**.</span><span class="sxs-lookup"><span data-stu-id="6a015-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

 ><span data-ttu-id="6a015-110">Åbn med Stifinder i SharePoint bruger ActiveX-objekter, så kommandoen understøttes kun i Internet Explorer 10 eller 11.</span><span class="sxs-lookup"><span data-stu-id="6a015-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="6a015-111">Åbn med Stifinder fungerer ikke i Windows med Microsoft Edge, Google Chrome, Mozilla Firefox eller på Mac-platformen.</span><span class="sxs-lookup"><span data-stu-id="6a015-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="6a015-112">Stifinder-visning kan af disse grunde være nedtonet.</span><span class="sxs-lookup"><span data-stu-id="6a015-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

> - <span data-ttu-id="6a015-113">[Hvorfor er knapperne til SharePoint-båndet ikke tilgængelige eller nedtonet?](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="6a015-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

