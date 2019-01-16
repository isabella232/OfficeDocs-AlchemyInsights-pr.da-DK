---
title: Adgangsbegrænsning i SharePoint- eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283063"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="86af8-102">Adgangsbegrænsning i SharePoint- eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="86af8-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="86af8-p101">I SharePoint- og OneDrive kan begrænse du adgangen til emner som filer, mapper og lister ved at give adgang til grupper eller enkeltpersoner, som du vil have adgang. Som standard nedarves tilladelser i SharePoint fra højere oppe i hierarkiet. Så en fil, der nedarver tilladelser fra den mappe, der nedarver tilladelser fra biblioteket, der nedarver tilladelser fra webstedet.</span><span class="sxs-lookup"><span data-stu-id="86af8-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="86af8-p102">Du kan dele på et højere niveau (f.eks ved at dele et helt websted) og derefter bryde nedarvningen, hvis du ikke ønsker at dele alle elementerne på webstedet. Dog anbefales ikke det fordi den gør vedligeholdelse tilladelserne mere kompleks og forvirrende i fremtiden. Her er, hvad du kan gøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="86af8-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="86af8-109">Hvis du vil dele indholdet af en mappe med undtagelse af én fil i det, skal du flytte filen til en ny placering, der ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="86af8-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="86af8-110">Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og kun gruppe A adgang til den anden undermappe, dele den overordnede mappe med gruppe A og gruppe B tilføjes i den første undermappe.</span><span class="sxs-lookup"><span data-stu-id="86af8-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="86af8-111">Stoppe deling af en fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="86af8-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

