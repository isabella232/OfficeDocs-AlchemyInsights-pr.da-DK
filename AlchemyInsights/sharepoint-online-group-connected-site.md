---
title: Føje en gruppe til et SharePoint websted
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897710"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Almindelige problemer ved oprettelse af et gruppeforbundet websted i SharePoint

1. Hvis du har slettet en gruppe og dens tilknyttede websted og ønsker at oprette et andet websted med den samme URL-adresse, skal du fjerne det forrige websted permanent.

   - Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Du kan finde flere oplysninger om at komme i gang med Powershell [under Introduktion SharePoint Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Fjern webstedet fra slettede websteder ved hjælp af [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell-cmdlet'en. PowerShell er påkrævet for at slette gruppewebsteder permanent.

1. Hvis du opretter et gruppeforbundet websted, og der vises en advarsel: Der findes allerede en anden gruppe med det samme **alias**, skal du kontrollere de eksisterende grupper [Microsoft 365 Administration](https://admin.microsoft.com/AdminPortal/Home#/groups). Du kan løse problemet ved at slette den eksisterende gruppe, hvis der ikke længere er brug for den, eller oprette webstedet med et andet alias tildelt.

1. Der er forskellige måder at oprette og bruge moderne grupper med SharePoint.

   - Du kan knytte eksisterende websteder til en Microsoft 365 gruppe. Du kan finde flere oplysninger [Forbind en Microsoft 365 gruppe, der bruger SharePoint brugergrænsefladen.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Hvis du vil Microsoft 365 websted med forbindelse til en gruppe, skal du oprette et [teamwebsted](https://admin.microsoft.com/sharepoint).
