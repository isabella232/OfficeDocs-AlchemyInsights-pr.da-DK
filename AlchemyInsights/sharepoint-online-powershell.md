---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764255"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Arbejder du med PowerShell eller Scripts i Sharepoint Online? Besøg nedenstående links for mere information.
- [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Oprette forbindelse til SPO PowerShell med multifaktorgodkendelse (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) indeholder et bibliotek med PowerShell-kommandoer, der giver dig mulighed for at udføre komplekse administrationshandlinger over for SPO.

> [!NOTE]
> - Hvis du har problemer med at oprette forbindelse til SPO-administrationsshell, skal du kontrollere, at du har opdateret til den nyeste version, og forsøge at [importere modulet igen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) ved hjælp af *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Hvis du forsøger at køre objektmodelscripts på klientsiden, skal [sharepoint onlineklientkomponenterne sDK'et](https://www.microsoft.com/download/details.aspx?id=42038) være installeret på den lokale computer.
> - Hvis du har problemer med at køre scripts fra PowerShell, kan du overveje at køre PowerShell som administrator og ændre [kørselspolitikken](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).