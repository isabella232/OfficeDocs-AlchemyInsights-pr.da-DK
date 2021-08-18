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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321855"
---
# <a name="open-with-explorer-isnt-working"></a>Åbn med Stifinder fungerer ikke

Hvis **Åbn med Stifinder** eller Vis i **Stifinder** ikke virker, skal du sørge for, at webklienttjenesten er indstillet til **Kører** ved at følge nedenstående trin. Det kan f.eks. tage lang tid at åbne et SharePoint eller OneDrive, når tjenesten ikke kører. 
  
1. I søgefeltet Windows skal du skrive Kør, vælge Kør skrivebordsapp, skrive services.msc og derefter vælge **Enter**.
    
2. Rul ned til WebClient-tjenesten, og markér **kolonnen Status.** Hvis WebClient-tjenestestatus ikke **kører,** skal du dobbeltklikke på tjenesten, klikke **på Start** og derefter klikke på **OK.** Aktivér tjenesten, hvis det er nødvendigt, ved at vælge **enten** **Manuel eller** Automatisk i **feltet Starttype.** 
    
**Bemærk!** Hvis du vil foretage fejlfinding af problemer med at åbne i Stifinder, skal [du se Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665). Udforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint filer med den nye OneDrive-synkronisering klient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

