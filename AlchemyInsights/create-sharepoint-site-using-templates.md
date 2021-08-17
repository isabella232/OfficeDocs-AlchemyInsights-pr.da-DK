---
title: Opret et websted i SharePoint Online
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057960"
---
# <a name="create-sharepoint-sites-using-templates"></a>Oprette SharePoint ved hjælp af skabeloner

Muligheden for at gemme et websted som en skabelon understøttes ikke med moderne Kommunikation eller Teamwebsteder. Du kan finde flere oplysninger om brug [af skabeloner under Gem, download og upload SharePoint websted som en skabelon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Her er nogle almindelige problemer/løsninger vedrørende lagring af et websted eller en liste som en skabelon i Sharepoint Online. 

**Knappen Gem websted/listeskabelon er ikke tilgængelig eller mangler**

Administratorer skal tillade brugerdefineret script for at aktivere skabelonfunktionerne. Du kan finde detaljerede trin, eksempler og overvejelser under 

- [Tillad eller forbyd brugerdefineret script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Gem websted som skabelon understøttes ikke og kan medføre problemer på websteder, der bruger SharePoint Server-publiceringsinfrastruktur.

**Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt**

Skabelonen mangler muligvis en [funktion og](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) aktiveres ikke. Hvis funktionen ikke er tilgængelig til aktivering i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen til at oprette et websted.

- Kontrollér, om der er lister [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) eller biblioteker, der overskrider grænseværdien for listevisning på 5.000 elementer, da dette kan blokere oprettelsen af en webstedsskabelon.

- Webstedet bruger muligvis for mange ressourcer, og derfor overskrider webstedsskabelonen grænsen på 50 MB.


- Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Få mere at vide [under Skabelongenereret liste viser ikke data fra den korrekte opslagsliste i SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Du kan finde flere oplysninger om almindelige problemer og løsninger i [Opret og brug webstedsskabeloner.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



