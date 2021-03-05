---
title: Problem med AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481464"
---
# <a name="problem-with-aad-connect-health"></a>Problem med AAD Connect Health

- Sørg for, at du har tilladelse til at udføre handlingen. Globale administratorer har som standard adgang. Desuden kan du bruge rollebaseret [adgangskontrol til at](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) uddelegere registreringstilladelse til bidragyderen.
- Sørg for, at de nødvendige slutpunkter er aktiveret og ikke blokeret på grund af firewallen. Du kan finde flere oplysninger under [krav.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registrering kan mislykkes, fordi udgående kommunikation bliver underlagt SSL-inspektion af netværkslaget.
- Sørg for, at du har bekræftet indstillingerne for meddelelser for Azure AD Connect Health. Gennemse din indstilling. Denne [vejledning kan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) hjælpe dig med at forstå, hvordan du konfigurerer meddelelsesindstillingerne for Azure AD Connect-tilstandsmeddelelser.
- Du kan få mere at vide om AAD Connect Health-synkroniseringsrapporten, og hvordan du henter den, i [rapporten Objektniveausynkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Hvis du vil foretage fejlfinding af AAD Connect Health-beskeder, skal du følge fejlfindingsvejledningen til beskeder om, hvor vigtige [AAD Connect Health-data](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) er, og om ofte stillede spørgsmål, skal du se almindelige [installationsspørgsmål om AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
