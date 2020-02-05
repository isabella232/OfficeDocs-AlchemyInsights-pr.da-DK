---
title: Oprette et websted i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770417"
---
# <a name="create-sharepoint-sites-using-templates"></a>Oprette SharePoint-websteder ved hjælp af skabeloner

Muligheden for at gemme et websted som skabelon understøttes ikke med moderne kommunikation eller teamwebsteder. Du kan finde flere oplysninger om brug af skabeloner under [Gem, downloade og overføre et SharePoint-websted som en skabelon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Her er nogle almindelige problemer/løsninger vedrørende lagring af et websted eller en liste som skabelon i Sharepoint Online. 

**Knappen Gem websteds-/listeskabelon er ikke tilgængelig eller mangler**

Administratorer skal tillade brugerdefineret script for at aktivere skabelonfunktionerne. For detaljerede trin, eksempler og overvejelser se 

- [Tillad eller forbyt brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Gem websted som skabelon understøttes ikke og kan give problemer på websteder, der bruger SharePoint Server Publishing Infrastructure.

**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**

Skabelonen mangler muligvis en [funktion](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke. Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.

- Kontroller, om lister eller biblioteker overskrider grænseværdien for grænseværdien for [listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer, da dette kan blokere oprettelsen af en webstedsskabelon.

- Webstedet bruger muligvis for mange ressourcer, og webstedsskabelonen overskrider derfor grænsen på 50 MB.


- Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Du kan finde flere oplysninger under [Listen Skabelongenererede vises ikke data fra den korrekte opslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Du kan finde flere oplysninger om almindelige problemer og løsninger ved at se [Oprette og bruge webstedsskabeloner](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



