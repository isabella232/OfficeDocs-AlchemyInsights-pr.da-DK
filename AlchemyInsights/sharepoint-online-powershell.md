---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709064"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Arbejder du med PowerShell eller scripts i Sharepoint Online? Gå til nedenstående links for at få flere oplysninger.
- [Introduktion til SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Opret forbindelse til SPO PowerShell med multifaktorgodkendelse (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) indeholder et bibliotek af PowerShell-kommandoer, der gør det muligt at udføre komplekse administrationshandlinger over for SPO.

> [!NOTE]
> - Hvis du har problemer med at oprette forbindelse til SPO management shell, skal [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) du sørge for, at du har opdateret til den nyeste version og prøve at importere modulet igen ved hjælp af *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Hvis du forsøger at køre scripts til objektmodeller på klientsiden, skal [Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) Client Components SDK være installeret på din lokale computer.
> - Hvis du har problemer med at køre scripts fra PowerShell, kan du overveje at køre PowerShell som administrator og ændre [eksekveringspolitikken.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)