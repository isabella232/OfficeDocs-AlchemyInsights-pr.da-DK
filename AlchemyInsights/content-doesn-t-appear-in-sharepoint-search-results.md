---
title: Indhold vises ikke i søgeresultater på SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517025"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Indhold vises ikke i søgeresultater på SharePoint

Følg disse fejlfindingstrin forventede indhold ikke vises i søgeresultater:
  
1. Kontroller, at det **websted** , der indeholder det forventede indhold er at tillade, at indholdet skal vises i søgeresultaterne. Følg trinnene i [Vis indhold på et websted i søgeresultaterne](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontroller, at den **liste** eller det **bibliotek** , der indeholder det forventede indhold er angivet til at tillade, at indholdet skal vises i søgeresultaterne. Følg trinnene i [Vis indhold fra lister eller biblioteker i søgeresultaterne](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontrollere, at den side, et dokument eller et brugerdefineret sidelayout er udgivet som en **hovedversion.** Følg trin 3 i [søgning returnerer ikke alle resultater i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontroller, at brugeren har **tilladelser** til at få vist indholdet. Følg trinnene på [forståelse af tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Hvis search-skema er blevet ændret, ved at tilføje en ny administreret egenskab, ved at redigere en administreret egenskab eller ved at fjerne en administreret egenskab, som derefter anmoder om en gennemsøgning og indeksere er påkrævet. **Indeksere** indholdet ved at følge trinnene i [manuelt anmode om gennemsøgning og indeksering igen af et websted, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Dette kan tage et stykke tid, vente 24 timer, før du kontrollerer resultaterne igen.

Yderligere oplysninger finder du under [aktivere indhold på et websted, der skal søges](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
