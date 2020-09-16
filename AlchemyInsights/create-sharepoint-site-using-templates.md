---
title: Oprette et websted i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732211"
---
# <a name="create-sharepoint-sites-using-templates"></a>Oprette SharePoint-websteder ved hjælp af skabeloner

Muligheden for at gemme et websted som en skabelon understøttes ikke med moderne kommunikations-eller team websteder. Du kan finde flere oplysninger om brug af skabeloner i [gemme, hente og overføre et SharePoint-websted som en skabelon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Her er nogle almindelige problemer/løsninger i forbindelse med at gemme et websted eller en liste som en skabelon i SharePoint Online. 

**Knappen Gem websted/listeskabelon er ikke tilgængelig eller mangler**

Administratorer skal tillade, at brugerdefineret script aktiverer skabelon funktionerne. Du kan finde detaljerede trin, eksempler og overvejelser i 

- [Tillade eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Gem websted som skabelon understøttes ikke og kan medføre problemer på websteder, der bruger SharePoint Server-publicerings infrastrukturen.

**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**

Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke. Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.

- Kontrollér, om lister eller biblioteker overskrider grænseværdien for [listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000-elementer, da dette kan blokere oprettelsen af en webstedsskabelon.

- Webstedet bruger muligvis for mange ressourcer, og derfor overskrider webstedsskabelonen grænsen på 50 MB.


- Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Hvis du vil have mere at vide, skal du se [listen skabelon oprettet viser ikke data fra den rigtige opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Du kan få mere at vide om almindelige problemer og løsninger ved [at se oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



