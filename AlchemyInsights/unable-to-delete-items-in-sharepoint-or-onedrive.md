---
title: Kan ikke slette elementer i SharePoint eller OneDrive
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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049511"
---
# <a name="unable-to-delete-items"></a>Kan ikke slette elementer

Har du problemer med at slette SharePoint-elementer?

- Sørg altid for, at du har de [nødvendige tilladelser](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) til at slette elementet eller få en administrator af en [gruppe af websteder](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) til at fjerne elementet.

- Kontroller, at der ikke er konfigureret en [opbevaringspolitik](https://docs.microsoft.com/office365/securitycompliance/retention-policies) for varen.

- Sørg for, at elementet ikke er [tjekket ud](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en anden bruger.

- Endelig kan administratorer bruge [SharePoint-mønstre og-praksisser](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), som indeholder et bibliotek med PowerShell-kommandoer, der giver dig mulighed for at udføre komplekse administrationshandlinger, f. eks.
- [Fjern PNP fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjern PNP-mappe](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjern PNP-listeelement](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjern PNP-liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjern PNP-felt (kolonne)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)