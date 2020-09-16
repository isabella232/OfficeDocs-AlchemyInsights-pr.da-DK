---
title: Gem websted eller liste som en skabelon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727525"
---
# <a name="save-site-or-list-as-a-template"></a>Gem websted eller liste som en skabelon

SharePoint-webstedsskabeloner er indbyggede definitioner, der er designet omkring et bestemt virksomheds behov. Du kan finde flere oplysninger i [brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er nogle almindelige problemer/løsninger i forbindelse med at gemme et websted eller en liste som en skabelon i SharePoint Online.

**Knappen Gem websted/listeskabelon er ikke tilgængelig eller mangler**. 

- Administratorer skal tillade, at brugerdefineret script aktiverer skabelon funktionerne. Du kan finde detaljerede trin, eksempler og overvejelser under [Tillad eller Forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Kommandoen Gem websted som skabelon understøttes ikke og kan medføre problemer på websteder, der bruger SharePoint Server-publicerings infrastrukturen.


**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**

- Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke. Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.


- Kontrollér, om lister eller biblioteker overskrider grænseværdien for [listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000-elementer, da dette kan blokere oprettelsen af en webstedsskabelon.


- Webstedet bruger muligvis for mange ressourcer, og webstedsskabelonen overskrider grænsen på 50 MB.


- Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Hvis du vil have mere at vide, skal du se [listen skabelon oprettet viser ikke data fra den rigtige opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Du kan få mere detaljerede oplysninger om almindelige problemer og løsninger ved [at oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

