---
title: Føje en gruppe til et SharePoint-websted
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771193"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemer ved oprettelse af et gruppe forbundet websted i SharePoint

1. Der opstod nogle almindelige problemer med at oprette eller genoprette en gruppes forbundne websted.
Hvis du har slettet en gruppe og den tilknyttede websted og vil oprette et andet websted med den samme URL-adresse, skal du fjerne det tidligere websted permanent.

   - Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Du kan finde flere oplysninger om at komme i gang med PowerShell i [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Fjernwebstedet fra slettede websteder ved hjælp af PowerShell [-cmdlet'en Fjern-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell kræves for at slette gruppe websteder permanent.

1. Hvis du opretter en gruppe forbundet websted og modtager en advarsel: der **findes allerede en gruppe med det samme alias**, skal du kontrollere de eksisterende grupper fra [Microsoft 365 administration](https://admin.microsoft.com/AdminPortal/Home#/groups). For at løse problemet skal du slette den eksisterende gruppe, hvis den ikke længere er nødvendig, eller oprette webstedet med et andet alias tildelt.

1. Der er forskellige måder at oprette og bruge moderne grupper på i SharePoint.

   - Du kan forbinde eksisterende websteder til en Microsoft 365-gruppe. Du kan finde flere oplysninger i [Opret forbindelse til en Microsoft 365-gruppe ved hjælp af SharePoint-brugergrænsefladen](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Hvis du vil oprette et Microsoft 365-gruppens forbundne websted, skal du oprette et [team websted](https://admin.microsoft.com/sharepoint).
