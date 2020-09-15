---
title: Indhold vises ikke i SharePoint-søgeresultater
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713124"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Indhold vises ikke i SharePoint-søgeresultater

Følg disse fejlfindingstrin, når det forventede indhold ikke vises i søgeresultaterne:
  
1. Kontrollér, at det **websted** , der indeholder det forventede indhold, er angivet til at tillade, at indhold vises i søgeresultaterne. Følg trinnene i [Vis indhold på et websted i søgeresultaterne](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontrollér, at den **liste** eller det **bibliotek** , der indeholder det forventede indhold, er angivet til at tillade, at indhold vises i søgeresultaterne. Følg trinnene i [Vis indhold fra lister eller biblioteker i søgeresultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontrollér, at side-, dokument-eller brugerdefineret sidelayout udgives som en over **ordnet version.** Følg trin 3 i [Søg returnerer ikke alle resultater i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontrollér, at brugeren har **tilladelse** til at få vist indholdet. Følg trinnene i [om tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Hvis søgeskemaet er blevet ændret ved at tilføje en ny administreret egenskab, ved at redigere en administreret egenskab eller ved at fjerne en administreret egenskab, vil det være nødvendigt at anmode om en gennemsøgning og et genindeks. **Indeksér indholdet igen** ved at følge trinnene i [manuelt gennemsøgning og Genindeksering af et websted, et bibliotek eller en liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Dette kan tage et stykke tid, vente 24 timer, før du tjekker resultaterne igen.

Hvis du vil have mere at vide, skal du se [aktivere indhold på et websted, der kan søges i](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
