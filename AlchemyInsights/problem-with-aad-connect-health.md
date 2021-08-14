---
title: Problem med AAD Forbind Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923746"
---
# <a name="problem-with-aad-connect-health"></a>Problem med AAD Forbind Health

- Sørg for, at du har tilladelse til at udføre handlingen. Globale administratorer har som standard adgang. Desuden kan du bruge [rollebaseret adgangskontrol til at](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) uddelegere registreringstilladelse til bidragyderen.
- Sørg for, at de nødvendige slutpunkter er aktiveret og ikke blokeret på grund af firewall. Du kan finde flere oplysninger i [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrering kan mislykkes, fordi udgående kommunikation bliver underlagt SSL-inspektion af netværkslaget.
- Sørg for, at du har bekræftet indstillingerne for meddelelser for Azure AD Forbind Tilstand. Gennemse din indstilling. Denne [vejledning](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) kan hjælpe dig med at forstå, hvordan du konfigurerer meddelelsesindstillingerne for Azure AD Forbind tilstandsmeddelelser.
- Du kan få mere at vide om rapporten AAD Forbind Health sync , og hvordan du henter den, under [Rapport over synkronisering på objektniveau](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Hvis du vil foretage fejlfinding af AAD Forbind Health-beskeder, skal du følge [fejlfindingsvejledningen til AAD Forbind Beskeder](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) om tilstandsdata og ofte stillede spørgsmål under Almindelige spørgsmål om installation af [AAD Forbind Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
