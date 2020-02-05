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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770345"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemer ved oprettelse af et gruppeforbundet websted i SharePoint

1. Nogle almindelige problemer opstod, når du opretter eller genopretter et gruppeforbundet websted.
Hvis du har slettet en gruppe og dens tilsluttede websted og ønsker at oprette et andet websted med den samme webadresse, skal du fjerne det forrige websted permanent.

   - Hent [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Du kan finde flere oplysninger om introduktion til Powershell under [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Fjern webstedet fra slettede websteder ved hjælp af cmdlet'en [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell er forpligtet til permanent at slette gruppewebsteder.

1. Hvis du opretter et gruppeforbundet websted og modtager en advarsel: Der findes allerede en **anden gruppe med det samme alias**, skal du kontrollere de eksisterende grupper fra Office [365 fra Administration](https://admin.microsoft.com/AdminPortal/Home#/groups). Du kan lÃ ̧se problemet ved at slette den eksisterende gruppe, hvis den ikke længere er nødvendig, eller oprette webstedet med et andet alias tildelt.

1. Der er forskellige måder at oprette og bruge moderne grupper på med SharePoint.

   - Du kan forbinde eksisterende websteder med en Office 365-gruppe. Du kan finde flere oplysninger under [Forbinde en Office 365-gruppe ved hjælp af SharePoint-brugergrænsefladen](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Hvis du vil oprette et Office 365-gruppe, der er tilsluttet websted, skal du oprette et [teamwebsted](https://admin.microsoft.com/sharepoint).
