---
title: Adgang nægtet, når du får vist en arbejdsproces
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688796"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Adgang nægtet, når du får vist en arbejdsproces

SharePoint 2013-arbejdsprocesser, der forsøger at sende en mail til en SharePoint-gruppe, kan mislykkes med fejlmeddelelsen "adgang nægtet", hvis medlemskabet af SharePoint-gruppen ikke er indstillet til alle.
  
 **Du kan løse dette problem ved at følge disse trin:**
  
 1. Tillad alle at se medlemmerne af SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra linjen til eller CC i mailen.
  
 3. Føj eksplicit brugere til til-eller CC-linjen, hvis medlemskabet af medlemskabet ikke kan ændres for SharePoint-gruppen.
  
Hvis du vil have mere at vide, skal du se [http-uautoriseret til/_vti_bin/Client.Svc/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  