---
title: AAD-meddelelser Forbind
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097300"
---
# <a name="notification-aad-connect"></a>AAD-meddelelser Forbind

- Sørg for, at du har tilladelse til at udføre handlingen. Globale administratorer har som standard adgang. Desuden kan du bruge [rollebaseret adgangskontrol til at](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) uddelegere registreringstilladelse til bidragyderen.
- Sørg for, at de nødvendige slutpunkter er aktiveret og ikke blokeret på grund af firewall. Du kan finde flere oplysninger i [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrering kan mislykkes, fordi udgående kommunikation bliver underlagt SSL-inspektion af netværkslaget.
- Sørg for, at du har bekræftet indstillingerne for meddelelser for Azure AD Forbind Tilstand, og gennemse din indstilling. Se denne vejledning for at få mere at vide om, hvordan du konfigurerer meddelelsesindstillingerne Forbind Azure AD Forbind [Tilstandsmeddelelser.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Du kan få mere at vide om rapporten AAD Forbind Health sync , og hvordan du henter den, under [Rapport over synkronisering på objektniveau](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Hvis du vil foretage fejlfinding af AAD Forbind Health Alerts, skal du følge [fejlfindingsvejledningen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) til vigtige beskeder om tilstand for AAD Forbind Health og for ofte stillede spørgsmål under Almindelige spørgsmål om [installation af AAD Forbind Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
