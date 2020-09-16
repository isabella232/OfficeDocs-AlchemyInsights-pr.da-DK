---
title: Foretag fejlfinding af "Åbn med Stifinder" i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ba9f11da5c35c3681e9bd5ceaf13233fe8b80fc9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737299"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="1722b-102">Foretag fejlfinding af "Åbn med Stifinder" i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1722b-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="1722b-103">Det anbefales, at du [synkroniserer SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), der giver mulighed for [Filer efter behov](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), fordi det giver lokal adgang til dine filer og den bedste ydeevne.</span><span class="sxs-lookup"><span data-stu-id="1722b-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="1722b-104">Følg trinnene og bedste praksis i følgende artikler for at fejlfinde problemer med Åbn med Stifinder:</span><span class="sxs-lookup"><span data-stu-id="1722b-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="1722b-105">Sådan bruger du kommandoen "Åbn med Stifinder" til at foretage fejlfinding af problemer i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1722b-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="1722b-106">Kopiér eller flyt biblioteksfiler ved hjælp af Åbn med Stifinder</span><span class="sxs-lookup"><span data-stu-id="1722b-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="1722b-107">**Bemærk!**</span><span class="sxs-lookup"><span data-stu-id="1722b-107">**Note:**</span></span>
>- <span data-ttu-id="1722b-108">Åbn med Stifinder understøttes kun i Internet Explorer 10 eller 11.</span><span class="sxs-lookup"><span data-stu-id="1722b-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="1722b-109">Åbn med Stifinder fungerer ikke i Windows med Microsoft Edge, Google Chrome, Mozilla Firefox eller på Mac-platformen.</span><span class="sxs-lookup"><span data-stu-id="1722b-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="1722b-110">Stifinder-visning kan af disse grunde være nedtonet.</span><span class="sxs-lookup"><span data-stu-id="1722b-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="1722b-111">Knappen Åbn med Stifinder vises ikke i den nye biblioteksoplevelse.</span><span class="sxs-lookup"><span data-stu-id="1722b-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="1722b-112">Vælg rullemenuen **Vis** øverst til højre (navnet på rullemenuen afhænger af, hvilken visning du i øjeblikket bruger), og vælg derefter **Vis i Stifinder**.</span><span class="sxs-lookup"><span data-stu-id="1722b-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
