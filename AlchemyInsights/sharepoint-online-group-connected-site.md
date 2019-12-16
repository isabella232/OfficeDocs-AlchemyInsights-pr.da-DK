---
title: Føje en gruppe til et SharePoint-websted
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051095"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemer ved oprettelse eller gruppe af tilknyttede websteder i SharePoint Online

Der er et par almindeligt forekommende problemer, når du opretter eller genopretter en gruppe forbundet websted.

 Hvis du har slettet en gruppe og dens tilsluttede websted og ønsker at oprette et andet websted med den samme webadresse, skal du fjerne det forrige websted permanent.

Hent [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Du kan finde flere oplysninger om, hvordan du kommer i gang med PowerShell, under [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Fjernwebstedet fra slettede websteder ved hjælp af [Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet.

Hvis du opretter et websted med tilknyttede websteder og modtager en advarsel om, at der allerede findes en anden gruppe med det samme alias, skal du kontrollere de eksisterende grupper fra [Office 365 fra administrationscenteret](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Du kan løse problemet ved at slette den eksisterende gruppe, hvis den ikke længere er nødvendig, eller oprette webstedet med et andet alias tildelt.

Der er forskellige måder at oprette og bruge moderne grupper med SharePoint.

Du kan oprette forbindelse mellem eksisterende websteder og en Office 365-gruppe. Du kan finde flere oplysninger under [oprette forbindelse fra en Office 365-gruppe ved hjælp af SharePoint-bruger ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Hvis du vil oprette et Office 365-gruppe tilsluttet websted, skal du oprette et team websted. Du kan finde flere oplysninger under [oprette et teamwebsted i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

