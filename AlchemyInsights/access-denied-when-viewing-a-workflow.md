---
title: Adgang nægtet, når du får vist en arbejdsproces
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28282513"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Adgang nægtet, når du får vist en arbejdsproces

SharePoint 2013 arbejdsprocesser, der forsøger at sende en e-mail til en SharePoint-gruppe kan mislykkes med en "Adgang nægtet"-fejlmeddelelse, hvis medlemskab af gruppen SharePoint ikke er indstillet til alle.
  
 **Du kan løse dette problem ved at gøre disse trin:**
  
 1. Gør det muligt for alle at se medlemmer af SharePoint-gruppen. 
  
 2. Fjern SharePoint-gruppen fra boksen til eller CC linje i e-mailen. 
  
 3. Tilføj brugerne eksplicit til til eller CC linje, hvis medlemskab synlighed ikke kan ændres for SharePoint-gruppe. 
  
For at få vist se flere oplysninger [HTTP med uautoriserede /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

