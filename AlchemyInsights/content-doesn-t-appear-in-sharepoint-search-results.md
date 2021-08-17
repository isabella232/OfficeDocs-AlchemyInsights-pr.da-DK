---
title: Indhold vises ikke i SharePoint søgeresultater
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
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081604"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Indhold vises ikke i SharePoint søgeresultater

Følg disse fejlfindingstrin, når det forventede indhold ikke vises i søgeresultaterne:
  
1. Kontrollér, at **webstedet,** der indeholder det forventede indhold, er indstillet til at tillade, at indhold vises i søgeresultater. Følg trinnene i [Vis indhold på et websted i søgeresultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontrollér, at **den liste** eller **det bibliotek,** der indeholder det forventede indhold, er indstillet til at tillade, at indhold vises i søgeresultater. Følg trinnene i [Vis indhold fra lister eller biblioteker i søgeresultater](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontrollér, at siden, dokumentet eller det brugerdefinerede sidelayout er publiceret som **en hovedversion.** Følg trin 3 [i Søg returnerer ikke alle resultater i SharePoint Online.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Kontrollér, at brugeren har **tilladelse til** at få vist indholdet. Følg trinnene i Forstå [tilladelsesniveauer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Hvis søgeskemaet er blevet ændret ved at tilføje en ny administreret egenskab, ved at redigere en administreret egenskab eller ved at fjerne en administreret egenskab, kræves der anmodning om en gennemsøgning og genindeksering. **Indekser indholdet** igen ved at følge trinnene i Anmod manuelt om gennemsøgning og genindeksering af et [websted, et bibliotek eller en liste.](https://docs.microsoft.com/sharepoint/crawl-site-content) Dette kan tage et stykke tid, vent 24 timer, før du kontrollerer resultaterne igen.

Du kan finde flere oplysninger i Aktivere søgbart indhold [på et websted.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
