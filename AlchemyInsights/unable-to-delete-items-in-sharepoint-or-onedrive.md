---
title: Elementer i SharePoint eller OneDrive kan ikke slettes
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511970"
---
# <a name="unable-to-delete-items"></a>Elementer kan ikke slettes

Opbevaringspolitikker kan forårsage dette, skal du enten deaktivere eller ekskludere respektive ventepositioner, der er årsag til dette problem. Når en opbevaringspolitik eller tilbageholdelse er fjernet, kan det tage op til 24 timer, før ændringen træder i kraft. Sørg for, at der ikke er oprettet en [opbevaringspolitik](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) for varen.

Webstedet kan have overskredet lagergrænsen, øget [webstedskvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) og slettet elementet.

Sørg for, at elementet ikke [er tjekket ud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en anden bruger.

Endelig kan administratorer bruge [PnP (SharePoint Patterns and Practices),](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) som indeholder et bibliotek med PowerShell-kommandoer, der giver dig mulighed for at udføre komplekse administrationshandlinger, f.eks.
- [Fjern PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjern pnp-listeelement](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjern PNP-felt (kolonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)