---
title: Gemme webstedet eller listen som en skabelon
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243239"
---
# <a name="save-site-or-list-as-a-template"></a>Gemme webstedet eller listen som en skabelon

SharePoint-websted-skabeloner er færdige definitioner, der er designet omkring et bestemt behov i virksomheden. Yderligere oplysninger finder du under [Brug af skabeloner til at oprette forskellige typer SharePoint-websteder](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er nogle almindelige problemer/løsninger med hensyn til lagring af et websted eller en liste som skabelon i SharePoint Online.

**Gem websted/denne liste skabelon knap er ikke tilgængelig eller mangler**. 

- Administratorer skal tillade brugerdefineret Script til at aktivere Skabelonfunktioner på. Se flere detaljerede oplysninger, eksempler og overvejelser i forbindelse med [Tillad eller forhindre brugerdefineret script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).


- Gem webstedet som skabelon-kommando understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-udgivelse-infrastruktur.


**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**

- Skabelonen mangler en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og kan ikke aktiveres. Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen for at oprette et websted.


- Kontrollere Hvis lister og biblioteker, overstiger den [Grænse for listevisning](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) af 5000 varer som dette kan blokere for oprettelse af en webstedsskabelon.


- Webstedet bruger måske for mange ressourcer, og derfor webstedsskabelonen overskrider grænsen på 50 MB (Megabyte).


- Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Yderligere oplysninger finder du i [skabelon-genereret liste ikke viser data fra den korrekte opslagsliste i SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


For mere detaljerede oplysninger om almindelige problemer og løsninger, skal du reference, [oprette og bruge webstedsskabeloner](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

