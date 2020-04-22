---
title: Åbn med Stifinder virker ikke
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713028"
---
# <a name="open-with-explorer-isnt-working"></a>Åbn med Stifinder fungerer ikke

Hvis **Åbn med Stifinder** eller **Vis i Stifinder** ikke virker, skal du sørge for, at webclient-tjenesten er indstillet til **Kørende** ved at følge nedenstående trin. det kan for eksempel tage lang tid at åbne et SharePoint- eller OneDrive-bibliotek, når tjenesten ikke kører. 
  
1. Skriv kør i søgefeltet i Windows, vælg appen Kør skrivebord, skriv services.msc, og vælg derefter **Enter**.
    
2. Rul ned til tjenesten WebClient, og kontroller kolonnen **Status.** Hvis webclient-tjenestestatus ikke **kører**, skal du dobbeltklikke på tjenesten, klikke på **Start**og derefter klikke på **OK**. Aktivér tjenesten, hvis det er nødvendigt, ved at vælge enten **Manuel** eller **Automatisk** i feltet **Starttype.** 
    
> [!NOTE]
> Hvis du vil foretage fejlfinding af problemer med at åbne i Stifinder, skal du se [Åbn i Stifinder](https://go.microsoft.com/fwlink/?linkid=871665). Udforsk synkronisering som et bedre alternativ: [Synkroniser SharePoint-filer med den nye OneDrive-synkroniseringsklient](https://go.microsoft.com/fwlink/?linkid=871666). 
  

