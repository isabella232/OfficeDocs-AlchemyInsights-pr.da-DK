---
title: Indhold vises ikke i SharePoint-søgeresultater
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705655"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Indhold vises ikke i SharePoint-søgeresultater

Følg disse fejlfindingstrin, når forventet indhold ikke vises i søgeresultater:
  
1. Kontroller, at det **websted,** der indeholder det forventede indhold, er indstillet til at tillade, at indhold vises i søgeresultaterne. Følg trinnene i [Vis indhold på et websted i søgeresultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontroller, at den **liste** eller det **bibliotek,** der indeholder det forventede indhold, er indstillet til at tillade, at indhold vises i søgeresultaterne. Følg trinnene i [Vis indhold fra lister eller biblioteker i søgeresultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontroller, at side-, dokument- eller brugerdefineret sidelayout udgives som en **Overordnet version.** Følg trin 3 i [Søg returnerer ikke alle resultater i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontroller, at brugeren har **tilladelse** til at få vist indholdet. Følg trinnene i [Om tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Hvis søgeskemaet er blevet ændret ved at tilføje en ny administreret egenskab, ved at redigere en administreret egenskab eller ved at fjerne en administreret egenskab, skal du anmode om et gennemsøgnings- og reindeks. **Indekser** indholdet igen ved at følge trinnene i [Manuel anmodning om gennemsøgning og reindeksering af et websted, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Dette kan tage et stykke tid, vent 24 timer, før du kontrollerer resultaterne igen.

Du kan finde flere oplysninger under [Aktivere, at indhold på et websted kan søges](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
