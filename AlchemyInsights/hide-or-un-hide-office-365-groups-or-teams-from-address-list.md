---
title: Skjul eller skjul Office 365-grupper eller teams fra adresselisten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811450"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skjul eller skjul Office 365-grupper eller teams fra adresselisten

Brug følgende EXO PowerShell-kommando til at skjule eller skjule Office 365-gruppe/teams fra adresselister (GAL) i Exchange-klienter (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Brug følgende EXO PowerShell-kommando til at skjule eller skjule Office365-gruppen/-teams fra Exchange-klienter (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Hvis du vil have detaljeret vejledning, [skal du se Skjul Office 365-grupper fra GAL og Exchange-klienter.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
