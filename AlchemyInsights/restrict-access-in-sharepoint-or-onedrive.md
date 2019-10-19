---
title: Begrænse adgangen i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551445"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrænse adgangen i SharePoint eller OneDrive

I SharePoint og OneDrive begrænser du adgangen til elementer som filer, mapper og lister ved kun at give adgang til grupper eller enkeltpersoner, du vil have adgang til. Tilladelser i SharePoint nedarves som standard fra højere op i hierarkiet. Så en fil arder sine tilladelser fra den mappe, som nedarer sine tilladelser fra biblioteket, som nedarer sine tilladelser fra webstedet.
  
Du kan dele på et højere niveau (f. eks. ved at dele et helt websted) og derefter afbryde nedarvning, hvis du ikke vil dele alle elementerne på webstedet. Men vi anbefaler ikke dette, fordi det gør opretholdelsen af tilladelserne mere komplekse og forvirrende i fremtiden. Her er, hvad du kan gøre i stedet:
  
- Hvis du for eksempel vil dele hele indholdet af en mappe med undtagelse af én fil i den, skal du flytte filen til en ny placering, der ikke er delt.
    
- Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og kun tillade gruppe adgang til den anden undermappe, skal du dele den overordnede mappe med gruppe A og tilføje gruppe B til den første undermappe.
    
[Stoppe delingen af en fil eller mappe](https://go.microsoft.com/fwlink/?linkid=2008861)
  

