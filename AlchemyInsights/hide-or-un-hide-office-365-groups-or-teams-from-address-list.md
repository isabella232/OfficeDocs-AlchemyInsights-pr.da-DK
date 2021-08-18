---
title: Skjul eller skjul Office 365 grupper eller teams fra adresselisten
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088390"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skjul eller skjul Office 365 grupper eller teams fra adresselisten

Brug følgende EXO PowerShell-kommando til at skjule eller skjule Office 365-gruppe/teams fra adresselister (GAL) i Exchange-klienter (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Brug følgende EXO PowerShell-kommando til at skjule eller skjule Office365-gruppen/-teams fra Exchange-klienter (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Du kan finde en detaljeret [vejledning under Skjul Office 365 grupper i GAL og Exchange klienter.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
