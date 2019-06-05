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
ms.openlocfilehash: 2097933dd20f326a7bda2151596d514c37d566ff
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717761"
---
# <a name="create-sharepoint-sites-using-templates"></a>Oprette SharePoint-websteder ved hjælp af skabeloner

SharePoint-websted-skabeloner er færdige definitioner, der er designet omkring et bestemt behov i virksomheden. Yderligere oplysninger finder du under <a href="https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4">ved hjælp af skabeloner til at oprette forskellige typer SharePoint-websteder.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Her er nogle almindelige problemer/løsninger med hensyn til lagring af et websted eller en liste som skabelon i Sharepoint Online.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Knappen Gem websted/denne liste skabelon er ikke tilgængelig eller mangler.</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Administratorer skal tillade brugerdefineret Script til at aktivere Skabelonfunktioner på. Se flere detaljerede oplysninger, eksempler og overvejelser i forbindelse med </span> </span> <a style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Tillad eller forhindre brugerdefineret script</a>.</li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Gem webstedet som skabelon-kommando understøttes ikke og kan forårsage problemer på websteder, der bruger SharePoint Server-udgivelse-infrastruktur.</span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Webstedsskabelonen kan ikke oprettes eller fungerer ikke korrekt</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Skabelonen mangler en <a href="https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx">funktion</a> og vandt&rsquo;t aktiver. Hvis funktionen ikke er tilgængelig til at aktivere i den aktuelle gruppe af websteder, kan du ikke bruge webstedsskabelonen for at oprette et websted.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Kontrollere Hvis lister og biblioteker, overstiger de <a href="https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59">Grænse for listevisning af</a> 5000 varer som dette kan blokere for oprettelse af en webstedsskabelon.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Webstedet bruger måske for mange ressourcer, og derfor webstedsskabelonen overskrider grænsen på 50 MB.</span></li> <li>
Der er problemer med at vise data fra en liste, der bruger en opslagskolonne. Yderligere oplysninger finder du i </span> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> <a style="box-sizing: border-box; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a"> <span style="color: #0067b8; text-decoration: none; text-underline: none;">skabelon-genereret liste&rsquo;t vises data fra den korrekte opslagsliste i SharePoint Online.

Yderligere oplysninger om almindelige problemer og løsninger, skal du kontrollere <a href="https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989">oprette og bruge webstedsskabeloner.



