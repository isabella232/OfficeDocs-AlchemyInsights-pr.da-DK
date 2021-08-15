---
title: Adgang nægtet ved visning af en arbejdsproces
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955195"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Adgang nægtet ved visning af en arbejdsproces

SharePoint 2013-arbejdsprocesser, der forsøger at sende en mail til en SharePoint-gruppe, kan mislykkes med fejlmeddelelsen "Adgang nægtet", hvis medlemskabet af SharePoint-gruppen ikke er angivet til Alle.
  
 **Du kan løse dette problem ved at udføre disse trin:**
  
 1. Tillad, at alle kan se medlemmer af SharePoint gruppe.
  
 2. Fjern SharePoint fra linjen Til eller Cc i mailen.
  
 3. Føj eksplicit brugerne til linjen Til eller Cc, hvis synligheden for medlemskab ikke kan ændres for SharePoint gruppe.
  
Hvis du vil have vist flere detaljer, skal du se HTTP uautoriseret [til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  