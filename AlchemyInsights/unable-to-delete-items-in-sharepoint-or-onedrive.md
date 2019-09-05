---
title: Kan ikke slette elementer i SharePoint eller OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748536"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="df63c-102">Kan ikke slette elementer</span><span class="sxs-lookup"><span data-stu-id="df63c-102">Unable to delete items</span></span>

<span data-ttu-id="df63c-103">Har du problemer med at slette SharePoint-elementer?</span><span class="sxs-lookup"><span data-stu-id="df63c-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="df63c-104">Sørg altid for, at du har de [nødvendige tilladelser](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) til at slette elementet eller få en administrator af en [gruppe af websteder](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) til at fjerne elementet.</span><span class="sxs-lookup"><span data-stu-id="df63c-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="df63c-105">Kontroller, at der ikke er konfigureret en [opbevaringspolitik](https://docs.microsoft.com/office365/securitycompliance/retention-policies) for varen.</span><span class="sxs-lookup"><span data-stu-id="df63c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="df63c-106">Sørg for, at elementet ikke er [tjekket ud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en anden bruger.</span><span class="sxs-lookup"><span data-stu-id="df63c-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="df63c-107">Endelig kan administratorer bruge [SharePoint-mønstre og-praksisser](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), som indeholder et bibliotek med PowerShell-kommandoer, der giver dig mulighed for at udføre komplekse administrationshandlinger, f. eks.</span><span class="sxs-lookup"><span data-stu-id="df63c-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="df63c-108">Fjern PNP fil</span><span class="sxs-lookup"><span data-stu-id="df63c-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="df63c-109">Fjern PNP-mappe</span><span class="sxs-lookup"><span data-stu-id="df63c-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="df63c-110">Fjern PNP-listeelement</span><span class="sxs-lookup"><span data-stu-id="df63c-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="df63c-111">Fjern PNP-liste</span><span class="sxs-lookup"><span data-stu-id="df63c-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="df63c-112">Fjern PNP-felt (kolonne)</span><span class="sxs-lookup"><span data-stu-id="df63c-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)