---
title: Oprette et websted i SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755302"
---
# <a name="create-sharepoint-sites-using-templates"></a>Oprette SharePoint-websteder ved hjælp af skabeloner

SharePoint-webstedsskabeloner er forudbyggede definitioner, der er designet omkring et bestemt forretningsbehov. Du finder flere oplysninger under [brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er nogle almindeligt forekommende problemer/løsninger vedrørende lagring af et websted eller en liste som en skabelon i SharePoint Online. 

**Knappen Gem websted/listeskabelon er ikke tilgængelig eller mangler**

Administratorer skal tillade brugerdefineret script for at aktivere skabelon funktionerne. Detaljerede trin, eksempler og overvejelser findes i 

- [Tillade eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Gem websted som skabelon understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-Publiceringsinfrastrukturen.

**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**

Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke. Hvis funktionen ikke er tilgængelig til aktivering i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.

- Kontroller, om lister eller biblioteker overskrider [grænse tærsklen på listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000 elementer, da dette kan blokere oprettelsen af en webstedsskabelon.

- Webstedet bruger muligvis for mange ressourcer, og webstedsskabelonen overskrider derfor grænsen på 50 MB.


- Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Du finder flere oplysninger under [skabelon genereret liste viser ikke data fra den korrekte opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Du kan finde mere detaljerede oplysninger om almindeligt forekommende problemer og løsninger ved at kontrollere [Opret og brug webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



