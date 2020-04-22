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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655276"
---
# <a name="data-location"></a>Placering af data

Du kan se placeringen af din lejer i Administration eller ved at oprette forbindelse til Exchange Online via PowerShell.


**Administration:**
1. Log på [Administration](https://admin.microsoft.com/Adminportal/Home).
2. Vælg**Organisationsprofil** **for indstillinger** > .
3. Vælg **Vis detaljer**under **Dataplacering**.


**Powershell:**
1. Opret forbindelse til Exchange Online ved hjælp af Windows PowerShell.
2. Udfør [cmdlet'en Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) for at få vist en liste over lejerens egenskaber. 
3. Kig på OrganizationId ejendom.

Når du har dataplaceringen for EXO og SPO, kan du bestemme dataplaceringen for andre tjenester, du kan bruge fra [det sted, hvor dine data er placeret.](https://products.office.com/where-is-your-data-located)