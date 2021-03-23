---
title: Meddelelse om AAD Connect
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
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035432"
---
# <a name="notification-aad-connect"></a>Meddelelse om AAD Connect

- Sørg for, at du har tilladelse til at udføre handlingen. Globale administratorer har som standard adgang. Desuden kan du bruge rollebaseret [adgangskontrol til at](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) uddelegere registreringstilladelse til bidragyderen.
- Sørg for, at de nødvendige slutpunkter er aktiveret og ikke blokeret på grund af firewall. Du kan finde flere oplysninger under [krav.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registrering kan mislykkes, fordi udgående kommunikation bliver underlagt SSL-inspektion af netværkslaget.
- Sørg for, at du har bekræftet indstillingerne for meddelelser for Azure AD Connect Health, og gennemse din indstilling. Se denne vejledning for at forstå, hvordan du konfigurerer meddelelsesindstillingerne for beskeder om Azure AD [Connect-tilstand.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- Hvis du vil have mere at vide om AAD Connect Health-synkroniseringsrapporten, og hvordan du henter den, skal du [se synkroniseringsrapporten på objektniveau.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Hvis du vil foretage fejlfinding af AAD Connect Health Alerts, skal du følge fejlfindingsvejledningen til beskeder om friskhed [for AAD Connect Health-data](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) og for ofte stillede spørgsmål under [Almindelige installationsspørgsmål om AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
