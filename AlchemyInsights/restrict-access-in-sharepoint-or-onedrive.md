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
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrænse adgangen i SharePoint eller OneDrive

I SharePoint og OneDrive begrænser du adgangen til emner som filer, mapper og lister ved kun at give adgang til grupper eller personer, du vil have adgang til. Tilladelser i SharePoint nedarves som standard højere oppe i hierarkiet. Så en fil arver sine tilladelser fra mappen, som arver sine tilladelser fra biblioteket, som arver dens tilladelser fra webstedet.
  
Du kan dele på et højere niveau (f.eks. ved at dele et helt websted) og derefter bryde nedarvningen, hvis du ikke vil dele alle elementerne på webstedet. Vi anbefaler dog ikke dette, fordi det gør det mere komplekst og forvirrende at vedligeholde tilladelserne i fremtiden. Her er, hvad du kan gøre i stedet:
  
- Hvis du for eksempel vil dele alt indholdet af en mappe med undtagelse af én fil i den, skal du flytte filen til en ny placering, der ikke deles.
    
- Hvis du har to undermapper i en mappe, og du vil dele en undermappe med gruppe A og B og kun tillade gruppe A-adgang til den anden undermappe, skal du dele den overordnede mappe med gruppe A og føje gruppe B til den første undermappe.
    
[Stoppe delingen af en fil eller mappe](https://go.microsoft.com/fwlink/?linkid=2008861)
  

