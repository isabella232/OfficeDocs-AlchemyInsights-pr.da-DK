---
title: Adgang nægtet ved visning af en arbejdsproces
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747742"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Adgang nægtet ved visning af en arbejdsproces

SharePoint 2013-arbejdsprocesser, der forsøger at sende en mail til en SharePoint-gruppe, kan mislykkes med en fejlmeddelelse af typen "adgang nægtet", hvis medlemskabet af SharePoint-gruppen ikke er angivet til alle.
  
 **Du kan løse dette problem ved at benytte følgende fremgangsmåde:**
  
 1. Tillad alle at se medlemmerne af SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra linjen til eller CC i e-mailen.
  
 3. Føj eksplicit brugerne til linjen til eller CC, hvis medlems synlighed ikke kan ændres for SharePoint-gruppen.
  
For at se flere oplysninger henvises til [http uautoriseret til/_vti_bin/Client.Svc/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  