---
title: Elementer i SharePoint eller OneDrive kunne ikke slettes
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571238"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="5ad6b-102">Elementer kan ikke slettes</span><span class="sxs-lookup"><span data-stu-id="5ad6b-102">Unable to delete items</span></span>

<span data-ttu-id="5ad6b-103">Opbevaringspolitikker kan forårsage dette, du skal enten deaktivere eller udelukke de respektive hold, der er årsag til dette problem.</span><span class="sxs-lookup"><span data-stu-id="5ad6b-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="5ad6b-104">Når en opbevaringspolitik eller tilbageholdelse er fjernet, kan det tage op til 24 timer, før ændringen træder i kraft.</span><span class="sxs-lookup"><span data-stu-id="5ad6b-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="5ad6b-105">Sørg for, at der ikke er konfigureret en opsætning af [opbevaringspolitik](https://docs.microsoft.com/office365/securitycompliance/retention-policies) på varen.</span><span class="sxs-lookup"><span data-stu-id="5ad6b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="5ad6b-106">Webstedet kan have overskredet lagergrænsen, forhøje [lokationskvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) og slette elementet.</span><span class="sxs-lookup"><span data-stu-id="5ad6b-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="5ad6b-107">Sørg for, at elementet ikke er [tjekket ud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en anden bruger.</span><span class="sxs-lookup"><span data-stu-id="5ad6b-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="5ad6b-108">Endelig kan administratorer bruge [PnP (SharePoint Patterns and Practices),](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) som indeholder et bibliotek med PowerShell-kommandoer, der giver dig mulighed for at udføre komplekse administrationshandlinger, f.eks.</span><span class="sxs-lookup"><span data-stu-id="5ad6b-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="5ad6b-109">Fjern PNP-fil</span><span class="sxs-lookup"><span data-stu-id="5ad6b-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="5ad6b-110">Fjern PNP-mappe</span><span class="sxs-lookup"><span data-stu-id="5ad6b-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="5ad6b-111">Fjern PNP-listeelement</span><span class="sxs-lookup"><span data-stu-id="5ad6b-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="5ad6b-112">Fjern PNP-liste</span><span class="sxs-lookup"><span data-stu-id="5ad6b-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="5ad6b-113">Fjern PNP-felt (kolonne)</span><span class="sxs-lookup"><span data-stu-id="5ad6b-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)