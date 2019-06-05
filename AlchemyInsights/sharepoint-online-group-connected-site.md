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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719476"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Opret gruppe forbundne websted i SharePoint Online

<p><strong>Der er et par almindelige problemer, der opstår, når forbundet websted, oprette eller genoprette en gruppe.&nbsp;</strong></p>  <p>1.Hvis du har slettet en gruppe og dets forbundne websted og ønsker at oprette et andet websted med samme URL-adresse, skal du fjerne det forrige websted permanent.</p>  <ul>  <li>Hent <a title="Simuleret administrationsshell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Simuleret Management Shell</a> - kan finde flere oplysninger under Introduktion til powershell i <a title="Introduktion til SharePoint Online administrationsshell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Introduktion til SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Fjern webstedet fra slettet websteder ved hjælp af den <a title="Fjern SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Fjern SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Hvis du opretter en gruppe forbundne websted og får vist en advarsel, <strong>'der findes en anden gruppe med det samme alias allerede'</strong>, kan du se de eksisterende grupper fra den <a title="Office 365 Admin-Center" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 Admin-Center</a>. Tildelt til at løse problemet, Slet den eksisterende gruppe, hvis det ikke længere er nødvendigt eller oprette webstedet med et andet alias.&nbsp;</p>  <p><strong>Der er forskellige måder at oprette og bruge moderne grupper med SharePoint.&nbsp;</strong></p>  <ol>  <li>Du kan oprette forbindelse til eksisterende websteder til Office 365-gruppen. Yderligere oplysninger finder du <a title="forbinde en Office 365-gruppe, ved hjælp af SharePoint bruger ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Oprette forbindelse til en Office 365-gruppe, ved hjælp af SharePoint bruger ineterface</a>.</li>  <li>Hvis du vil oprette et Office 365 gruppe forbundne websted, skal du oprette et websted for Team. Yderligere oplysninger finder du <a title="opretter et teamwebsted i SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Oprette et websted for team i SharePoint.</a></li>  </ol>

