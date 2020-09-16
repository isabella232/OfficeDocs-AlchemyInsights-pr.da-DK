---
title: Begræns adgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720676"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="28976-102">Begræns adgang i SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="28976-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="28976-103">I SharePoint og OneDrive kan du begrænse adgangen til elementer som filer, mapper og lister ved kun at give adgang til grupper eller enkeltpersoner, du vil have adgang til.</span><span class="sxs-lookup"><span data-stu-id="28976-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="28976-104">Tilladelser i SharePoint nedarves som standard fra mere i hierarkiet.</span><span class="sxs-lookup"><span data-stu-id="28976-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="28976-105">Så en fil arver dens tilladelser fra mappen, hvilket nedarver dens tilladelser fra biblioteket, som nedarver tilladelserne fra webstedet.</span><span class="sxs-lookup"><span data-stu-id="28976-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="28976-106">Du kan dele på et højere niveau (f. eks ved at dele et helt websted) og derefter bryde nedarvningen, hvis du ikke vil dele alle elementerne på webstedet.</span><span class="sxs-lookup"><span data-stu-id="28976-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="28976-107">Vi anbefaler dog ikke dette, da det gør det mere komplekst og forvirrende at være mere komplekst.</span><span class="sxs-lookup"><span data-stu-id="28976-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="28976-108">Du kan gøre følgende i stedet:</span><span class="sxs-lookup"><span data-stu-id="28976-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="28976-109">Hvis du f. eks vil dele alt indholdet af en mappe med undtagelse af en fil, skal du flytte filen til en ny placering, der ikke er delt.</span><span class="sxs-lookup"><span data-stu-id="28976-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="28976-110">Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupperne A og B og kun tillade gruppering af en adgang til den anden undermappe, kan du dele den overordnede mappe med gruppe A og tilføje gruppe B i den første undermappe.</span><span class="sxs-lookup"><span data-stu-id="28976-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="28976-111">Stoppe med at dele en fil eller mappe </span><span class="sxs-lookup"><span data-stu-id="28976-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

