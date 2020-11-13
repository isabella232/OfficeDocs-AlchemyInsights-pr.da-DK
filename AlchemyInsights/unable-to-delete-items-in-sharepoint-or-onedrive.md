---
title: Kan ikke slette elementer i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019577"
---
# <a name="unable-to-delete-items"></a>Kan ikke slette elementer

- Opbevaringspolitikker kan medføre dette, du skal enten deaktivere eller udelade den venteposition, der forårsager dette problem. Når en opbevaringspolitik eller-spærring fjernes, kan det tage op til 24 timer, før ændringen træder i kraft. Sørg for, at der ikke er konfigureret en [opbevaringspolitik](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) for elementet.

- Webstedet kan have overskredet lagergrænsen, øge [webstedets kvote](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) og slette elementet.

- Sørg for, at elementet ikke er [tjekket ud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en anden bruger.

- Endelig kan administratorer bruge [SharePoint-mønstre og-metoder](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) , der indeholder et bibliotek med PowerShell-kommandoer, som gør det muligt at udføre komplekse administrationshandlinger som f. eks. Gennemtving sletning af Stubborn-elementer.
- [Fjern PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjern PNP-listeelement](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjern PNP-felt (kolonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)