---
title: Slutpunkt DLP ikke installeret på brugerens enhed
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731408"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Slutpunkt DLP ikke installeret på brugerens enhed

Hvis indstillingen til forebyggelse af datatab på slutpunkter (DLP) ikke er anvendt på en brugers enhed, skal du bekræfte, at du opfylder følgende krav:

- Windows 10 x64 build 1809 eller nyere installeres på enheden.
- Antimalware-klientversion 4.18.2009.7 eller nyere installeres.
- Enheden er **en af** følgende:
    
    - Azure Active Directory (Azure AD) forbundet
    - Hybrid Azure AD forbundet
    - AAD registreret

- Hvis du vil gennemtvinge politikhandlinger, skal du sørge for, at Microsoft Chromium Edge-browseren er installeret på slutpunktsenheden.

Du kan finde yderligere krav til implementering af Endpoint DLP i Introduktion til [forebyggelse af datatab i slutpunkt.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)