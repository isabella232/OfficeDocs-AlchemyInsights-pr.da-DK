---
title: Adgang nægtet ved visning af en arbejdsproces
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687324"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Adgang nægtet ved visning af en arbejdsproces

SharePoint 2013-arbejdsprocesser, der forsøger at sende en mail til en SharePoint-gruppe, kan mislykkes med fejlmeddelelsen "Adgang nægtet", hvis medlemskabet af SharePoint-gruppen ikke er angivet til Alle.
  
 **Du kan lÃ ̧se problemet ved at benytte disse trin:**
  
 1. Giv alle mulighed for at se medlemmerne af SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra linjen Til eller CC i mailen.
  
 3. Føj eksplicit brugerne til linjen Til eller CC, hvis synligheden af medlemskabet ikke kan ændres for SharePoint-gruppen.
  
Du kan få vist flere oplysninger ved at se [HTTP Uautoriseret til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  