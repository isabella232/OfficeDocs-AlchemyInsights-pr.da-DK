---
title: Åbn med Stifinder virker ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538460"
---
# <a name="open-with-explorer-isnt-working"></a>Åbn med Stifinder fungerer ikke

Kontroller, at tjenesten WebClient er indstillet til at **køre** ved at benytte følgende fremgangsmåde, hvis **Åbn med Stifinder** eller **visning i File Explorer** ikke virker. For eksempel kan det tage lang tid at åbne et SharePoint- eller OneDrive-bibliotek, når tjenesten ikke kører. 
  
1. I feltet Windows Søg type Kør, Vælg Kør desktop app, skriv services.msc, og vælg derefter **Enter**.
    
2. Rul ned til tjenesten WebClient, og se i kolonnen **Status** . Hvis status for tjenesten WebClient ikke er **kører**, dobbeltklik på tjenesten, klikke på **Start**og derefter klikke på **OK**. Aktivere tjenesten, hvis det er nødvendigt, ved at vælge enten **Manuel** eller **automatisk** i **boksen** . 
    
> [!NOTE]
> Hvis du vil foretage fejlfinding af problemer, der er åbne i Filoversigt, se [åbne i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Udforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive sync-klient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

