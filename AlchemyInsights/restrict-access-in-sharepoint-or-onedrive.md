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
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075034"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begræns adgang i SharePoint eller OneDrive

I SharePoint og OneDrive kan du begrænse adgangen til elementer som filer, mapper og lister ved kun at give adgang til grupper eller enkeltpersoner, du vil have adgang til. Som standard nedarves tilladelser i SharePoint oppefra og op i hierarkiet. Derfor nedarver en fil sine tilladelser fra mappen, som nedarver dens tilladelser fra biblioteket, som nedarver dens tilladelser fra webstedet.
  
Du kan dele på et højere niveau (f.eks. ved at dele et helt websted) og derefter bryde nedarvningen, hvis du ikke vil dele alle elementerne på webstedet. Vi anbefaler dog ikke dette, da det gør vedligeholdelsen af tilladelserne mere kompleks og forvirrende i fremtiden. Her er, hvad du kan gøre i stedet:
  
- Hvis du f.eks. vil dele alt indholdet i en mappe undtagen én fil i den, skal du flytte filen til en ny placering, der ikke er delt.
    
- Hvis du har to undermapper i en mappe, og du vil dele én undermappe med gruppe A og B og kun tillade gruppe A adgang til den anden undermappe, skal du dele den overordnede mappe med gruppe A og føje gruppe B til den første undermappe.
    
[Stop delingen af en fil eller mappe ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

