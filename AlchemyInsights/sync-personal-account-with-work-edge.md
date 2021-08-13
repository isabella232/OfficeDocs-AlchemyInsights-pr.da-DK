---
title: Gør det muligt for en bruger at synkronisere en personlig konto med arbejdskontoen i Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813392"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Gør det muligt for en bruger at synkronisere en personlig konto med arbejdskontoen i Microsoft Edge

Sørg for, at du opfylder disse kriterier:

- Enterprise State Roaming er aktiveret i Azure Active Directory Administration, hvilket kræver et abonnement på Azure Active Directory Premium eller Enterprise Mobility + Security (EMS). Du kan finde flere oplysninger [i Aktivere Enterprise State Roaming i Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Et eller begge af følgende kriterier er opfyldt:
    - Azure Information Protection-tjenesten er aktiveret for din lejer. Du kan få mere at [vide under Aktivere Azure Rights Management-beskyttelse fra Microsoft 365 Administration](/azure/information-protection/activate-office365).
    - Funktionen Azure Active Directory Enterprise State Roaming (ESR) er aktiveret for alle brugere eller lejere. Du kan få mere at vide [under Hvad er virksomhedsamaming?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Hvis både AIP og ESR er deaktiveret, informerer en fejlmeddelelse brugerne om, at synkronisering ikke er tilgængelig for deres konti.
