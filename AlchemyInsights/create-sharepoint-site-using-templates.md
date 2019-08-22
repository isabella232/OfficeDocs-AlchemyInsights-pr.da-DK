---
title: Oprette et websted i SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514992"
---
# <a name="create-sharepoint-sites-using-templates"></a>Oprette SharePoint-websteder ved hjælp af skabeloner

SharePoint-websted-skabeloner er færdige definitioner, der er designet omkring et bestemt behov i virksomheden. Yderligere oplysninger finder du under [Brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er nogle almindelige problemer/løsninger med hensyn til lagring af et websted eller en liste som skabelon i Sharepoint Online. 

**Knappen Gem websted/denne liste skabelon er ikke tilgængelig eller mangler**

Administratorer skal tillade brugerdefineret Script til at aktivere Skabelonfunktioner på. Se for detaljerede trin, eksempler og overvejelser 

- [Tillade eller forhindre brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Gem webstedet som skabelon-kommando understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-udgivelse-infrastruktur.

**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**

Skabelonen mangler en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og kan ikke aktiveres. Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen for at oprette et websted.

- Kontrollere Hvis lister og biblioteker, overstiger den [Grænse for listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) af 5000 varer som dette kan blokere for oprettelse af en webstedsskabelon.

- Webstedet bruger måske for mange ressourcer, og derfor webstedsskabelonen overskrider grænsen på 50 MB.


- Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Yderligere oplysninger finder du i [skabelon-genereret liste ikke viser data fra den korrekte opslagsliste i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Mere detaljerede oplysninger om almindelige problemer og løsninger, skal du kontrollere [oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



