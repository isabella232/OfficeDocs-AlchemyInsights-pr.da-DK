---
title: Vejledning i at skjule/vise en gruppe fra adresselisten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926239"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skjule Microsoft 365 gruppe fra adresselisten (GAL)

Hvis du vil skjule Microsoft 365 gruppe fra adresselisterne (GAL) Exchange-klienter (f.eks. Outlook eller OWA), skal du bruge følgende kommando i EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Hvis du vil skjule Microsoft 365 gruppe, så den ikke er synlig Exchange kunder, skal du bruge følgende kommando i EXO-shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

