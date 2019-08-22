---
title: Adgang nægtet, når du får vist en arbejdsproces
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495817"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Adgang nægtet, når du får vist en arbejdsproces

SharePoint 2013 arbejdsprocesser, der forsøger at sende en e-mail til en SharePoint-gruppe kan mislykkes med en "Adgang nægtet"-fejlmeddelelse, hvis medlemskab af gruppen SharePoint ikke er indstillet til alle.
  
 **Du kan løse dette problem ved at gøre disse trin:**
  
 1. Gør det muligt for alle at se medlemmer af SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra boksen til eller CC linje i e-mailen.
  
 3. Tilføj brugerne eksplicit til til eller CC linje, hvis medlemskab synlighed ikke kan ændres for SharePoint-gruppe.
  
For at få vist se flere oplysninger [HTTP med uautoriserede /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  