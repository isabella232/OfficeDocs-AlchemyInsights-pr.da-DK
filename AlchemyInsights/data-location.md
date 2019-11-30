---
title: Placering af data
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627840"
---
# <a name="data-location"></a>Placering af data

Du kan få vist placeringen af din Office 365-lejer i administrationscenteret eller ved at oprette forbindelse til Exchange Online via PowerShell.


**Admin Center:**
1. Log på [Admin Center](https://admin.microsoft.com/Adminportal/Home).
2. Vælg **Indstillinger** > **organisations profil**.
3. Vælg **Vis detaljer**under **data placering**.


**Powershell:**
1. Opret forbindelse til Exchange Online ved hjælp af Windows PowerShell.
2. Kør cmdlet'en [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for at få vist en liste over din lejer egenskaber. 
3. Se på egenskaben OrganizationId.

Når du har dataplaceringen for EXO og SPO, kan du bestemme dataplaceringen for andre tjenester, du kan bruge, fra [hvor dine data er placeret](https://products.office.com/where-is-your-data-located).