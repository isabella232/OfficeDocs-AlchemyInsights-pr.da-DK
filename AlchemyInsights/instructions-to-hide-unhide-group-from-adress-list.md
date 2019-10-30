---
title: Instruktioner til Skjul/Vis gruppe fra adresseliste
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768910"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Skjul Office 365 gruppe fra adresseliste (GAL)

Hvis du vil skjule en Office 365-gruppe fra adresselister (GAL) for Exchange-klienter (f. eks. Outlook eller OWA), skal du bruge følgende kommando i EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Hvis du vil skjule Office 365-gruppen, så den ikke er synlig for Exchange-klienter, skal du bruge følgende kommando i EXO shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

