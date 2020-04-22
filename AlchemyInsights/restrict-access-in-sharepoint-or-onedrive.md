---
title: Begrænse adgangen i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715878"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="be635-102">Begrænse adgangen i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="be635-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="be635-103">I SharePoint og OneDrive begrænser du adgangen til emner som filer, mapper og lister ved kun at give adgang til grupper eller personer, du vil have adgang til.</span><span class="sxs-lookup"><span data-stu-id="be635-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="be635-104">Tilladelser i SharePoint nedarves som standard højere oppe i hierarkiet.</span><span class="sxs-lookup"><span data-stu-id="be635-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="be635-105">Så en fil arver sine tilladelser fra mappen, som arver sine tilladelser fra biblioteket, som arver dens tilladelser fra webstedet.</span><span class="sxs-lookup"><span data-stu-id="be635-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="be635-106">Du kan dele på et højere niveau (f.eks. ved at dele et helt websted) og derefter bryde nedarvningen, hvis du ikke vil dele alle elementerne på webstedet.</span><span class="sxs-lookup"><span data-stu-id="be635-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="be635-107">Vi anbefaler dog ikke dette, fordi det gør det mere komplekst og forvirrende at vedligeholde tilladelserne i fremtiden.</span><span class="sxs-lookup"><span data-stu-id="be635-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="be635-108">Her er, hvad du kan gøre i stedet:</span><span class="sxs-lookup"><span data-stu-id="be635-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="be635-109">Hvis du for eksempel vil dele alt indholdet af en mappe med undtagelse af én fil i den, skal du flytte filen til en ny placering, der ikke deles.</span><span class="sxs-lookup"><span data-stu-id="be635-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="be635-110">Hvis du har to undermapper i en mappe, og du vil dele en undermappe med gruppe A og B og kun tillade gruppe A-adgang til den anden undermappe, skal du dele den overordnede mappe med gruppe A og føje gruppe B til den første undermappe.</span><span class="sxs-lookup"><span data-stu-id="be635-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="be635-111">Stoppe delingen af en fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="be635-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

