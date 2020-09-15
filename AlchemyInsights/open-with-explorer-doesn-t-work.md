---
title: Åbn med Stifinder virker ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694450"
---
# <a name="open-with-explorer-isnt-working"></a>Åbn med Stifinder fungerer ikke

Hvis **Åbn med Stifinder** eller **Vis i Stifinder** ikke fungerer, skal du sikre dig, at WebClient-tjenesten er indstillet til at **køre** ved at følge nedenstående trin. For eksempel kan det tage lang tid at åbne et SharePoint-eller OneDrive-bibliotek, når tjenesten ikke kører. 
  
1. Skriv Kør i feltet Windows Search, Vælg appen Kør skrivebord, skriv Services. msc, og vælg derefter **Enter**.
    
2. Rul ned til tjenesten Webklient, og Markér kolonnen **status** . Hvis WebClient-Tjenestestatus ikke **kører**, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**. Aktivér tjenesten, hvis det er nødvendigt, ved at vælge enten **manuelt** eller **automatisk** i feltet **starttype** . 
    
> [!NOTE]
> Hvis du vil foretage fejlfinding af problemer, der åbnes i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665). Udforsk Synkroniser som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

