---
title: Føje en gruppe til et SharePoint-websted
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758725"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Opret gruppe forbundne websted i SharePoint Online

Der er et par almindelige problemer, der opstår, når forbundet websted, oprette eller genoprette en gruppe.

 Hvis du har slettet en gruppe og dets forbundne websted og ønsker at oprette et andet websted med samme URL-adresse, skal du fjerne det forrige websted permanent.

Hent [Simuleret administrationsshell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Se [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) for at få flere oplysninger på Introduktion til powershell

Fjern webstedet fra slettet websteder ved hjælp af [Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.

Hvis du opretter en gruppe forbundne websted, og du modtager en advarsel, der findes allerede en anden gruppe med det samme alias, kan du se de eksisterende grupper fra [Office 365 Admin-Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Tildelt til at løse problemet, Slet den eksisterende gruppe, hvis det ikke længere er nødvendigt eller oprette webstedet med et andet alias.

Der er forskellige måder at oprette og bruge moderne grupper med SharePoint.

Du kan oprette forbindelse til eksisterende websteder til Office 365-gruppen. Du kan finde flere oplysninger, skal [Tilslut en Office 365-gruppe, ved hjælp af SharePoint bruger ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Hvis du vil oprette et Office 365 gruppe forbundne websted, skal du oprette et websted for Team. For yderligere oplysninger se [oprette et websted for team i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

