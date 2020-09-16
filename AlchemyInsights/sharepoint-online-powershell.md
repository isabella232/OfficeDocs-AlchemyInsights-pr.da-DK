---
title: SharePoint Online PowerShell
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770833"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Arbejder du med PowerShell eller scripts i SharePoint Online? Gå til linkene nedenfor for at få flere oplysninger.
- [Kom godt i gang med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Opret forbindelse til SPO PowerShell med multifaktorgodkendelse (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint-mønstre og-metoder (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) indeholder et bibliotek med PowerShell-kommandoer, der gør det muligt at udføre komplekse administrationshandlinger mod SPO.

> [!NOTE]
> - Hvis du har problemer med at oprette forbindelse til SPO Management Shell, skal du kontrollere, at du har opdateret til den nyeste version og forsøge at [importere modulet igen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) ved hjælp af *"import-modul Microsoft. online. SharePoint. PowerShell".*
> - Hvis du forsøger at køre script scripts på klientsiden, skal du have installeret [SDK som SharePoint Online-klientkomponenter](https://www.microsoft.com/download/details.aspx?id=42038) på din lokale computer.
> - Hvis du har problemer med at køre scripts fra PowerShell, kan det være en god ide at køre PowerShell som administrator og ændre [udførelses politikken](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).