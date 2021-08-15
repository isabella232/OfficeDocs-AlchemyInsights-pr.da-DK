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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011330"
---
# <a name="open-with-explorer-isnt-working"></a>Åbn med Stifinder fungerer ikke

Hvis **Åbn med Stifinder** eller Vis i **Stifinder** ikke virker, skal du sørge for, at webklienttjenesten er indstillet til **Kører** ved at følge nedenstående trin. Det kan f.eks. tage lang tid at åbne et SharePoint eller OneDrive, når tjenesten ikke kører. 
  
1. I søgefeltet Windows skal du skrive Kør, vælge Kør skrivebordsapp, skrive services.msc og derefter vælge **Enter**.
    
2. Rul ned til WebClient-tjenesten, og markér **kolonnen Status.** Hvis WebClient-tjenestestatus ikke **kører,** skal du dobbeltklikke på tjenesten, klikke **på Start** og derefter klikke på **OK.** Aktivér tjenesten, hvis det er nødvendigt, ved at vælge **enten** Manuel **eller** Automatisk **i feltet Starttype.** 
    
> [!NOTE]
> Hvis du vil foretage fejlfinding af problemer med at åbne i Stifinder, [skal du se Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665). Udforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint filer med den nye OneDrive-synkronisering klient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

