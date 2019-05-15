---
title: Kunne ikke slette elementer på SharePoint- eller OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057692"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="882f6-102">Kunne ikke slette elementer</span><span class="sxs-lookup"><span data-stu-id="882f6-102">Unable to delete items</span></span>

<span data-ttu-id="882f6-103">Har du problemer med at slette emner?</span><span class="sxs-lookup"><span data-stu-id="882f6-103">Having issues deleting items?</span></span>

- <span data-ttu-id="882f6-104">Kontroller altid, at du har de [nødvendige tilladelser](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) til at slette varen eller har et [webstedsadministrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) forsøg på at fjerne elementet.</span><span class="sxs-lookup"><span data-stu-id="882f6-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="882f6-105">Sørg for, at der ikke er en [opbevaringspolitik](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) opsætning på varen.</span><span class="sxs-lookup"><span data-stu-id="882f6-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="882f6-106">Sikre, at varen ikke er [tjekket ud](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en anden bruger.</span><span class="sxs-lookup"><span data-stu-id="882f6-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="882f6-107">Endelig kan administratorer bruge [SharePoint mønstre og praksis](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) der indeholder et bibliotek af PowerShell-kommandoer, der gør det muligt at udføre komplekse management handlinger som f.eks gennemtvinge sletning af stubborn elementer.</span><span class="sxs-lookup"><span data-stu-id="882f6-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="882f6-108">Fjerne Plug and Play-fil</span><span class="sxs-lookup"><span data-stu-id="882f6-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="882f6-109">Fjerne Plug and Play-mappe</span><span class="sxs-lookup"><span data-stu-id="882f6-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="882f6-110">Fjerne Plug and Play-listeelement</span><span class="sxs-lookup"><span data-stu-id="882f6-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="882f6-111">Fjerne Plug and Play-liste</span><span class="sxs-lookup"><span data-stu-id="882f6-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="882f6-112">Fjerne Plug and Play-felt (kolonne)</span><span class="sxs-lookup"><span data-stu-id="882f6-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)