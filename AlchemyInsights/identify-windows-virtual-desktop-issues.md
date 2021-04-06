---
title: Identificer problemer med virtuelt skrivebord i Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595514"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identificer problemer med virtuelt skrivebord i Windows

Windows Virtual Desktop Diagnostics bruger kun én PowerShell-cmdlet, men indeholder mange valgfrie parametre til at indskrænke og isolere problemer. Sådan kommer du i gang: 

1. Download og importér Windows Virtual Desktop PowerShell-modulet. Du kan finde flere oplysninger [i Windows Virtual Desktop Cmdlet'er til Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Kør følgende cmdlet for at logge på din konto:
    
    Eksempel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**BEMÆRK!** Alle forespørgsler, der bruger PowerShell, skal indeholde parametrene -UserName eller -ActivityID. Du kan finde overvågningsegenskaber under [Brug Loganalyse til diagnosticeringsfunktionen.](https://go.microsoft.com/fwlink/?linkid=2126847)

Hvis du vil filtrere diagnosticeringsaktiviteter efter bruger, skal du køre følgende cmdlet:

Eksempel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Der er en liste over filtre, du kan køre for at diagnosticere problemer. Du kan få mere at vide om diagnosticering af problemer under [Identificere og diagnosticere problemer med virtuel skrivebord i Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Hvis du vil have mere at vide om almindelige fejl, skal du se Almindelige fejl [senarios.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
