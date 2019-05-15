---
title: Kunne ikke slette elementer på SharePoint- eller OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057692"
---
# <a name="unable-to-delete-items"></a>Kunne ikke slette elementer

Har du problemer med at slette emner?

- Kontroller altid, at du har de [nødvendige tilladelser](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) til at slette varen eller har et [webstedsadministrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) forsøg på at fjerne elementet.

- Sørg for, at der ikke er en [opbevaringspolitik](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) opsætning på varen.

- Sikre, at varen ikke er [tjekket ud](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) til en anden bruger.

- Endelig kan administratorer bruge [SharePoint mønstre og praksis](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) der indeholder et bibliotek af PowerShell-kommandoer, der gør det muligt at udføre komplekse management handlinger som f.eks gennemtvinge sletning af stubborn elementer. 
- [Fjerne Plug and Play-fil](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Fjerne Plug and Play-mappe](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Fjerne Plug and Play-listeelement](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Fjerne Plug and Play-liste](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Fjerne Plug and Play-felt (kolonne)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)