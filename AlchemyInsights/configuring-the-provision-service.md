---
title: Konfiguration af klargøringstjenesten
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
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033272"
---
# <a name="configuring-the-provision-service"></a>Konfiguration af klargøringstjenesten

For at automatisere bruger klargøring kan fungere, kræver Azure AD gyldige legitimationsoplysninger, der giver mulighed for at oprette forbindelse til Workday Web Services API. Desuden valideres knappen Test forbindelse på appen Klargøring af arbejdsdag til AD-bruger også, om den kan oprette forbindelse til Den Azure AD Forbind-klargøringsagent, der er knyttet til AD-domænet.

Hvis Azure-portalen returnerer en fejl, når du gemmer legitimationsoplysningerne, skal du følge de anbefalede trin nedenfor:

1. Bekræft, at du har konfigureret arbejdsdagens integrationssystembrugerkonto som nævnt i selvstudiet Om [konfiguration af integrationssystembruger i Arbejdsdag.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Bekræft, at Azure AD Forbind Provisioning Agent Service er i gang med at køre på din lokale Windows server ved hjælp af Services Management Console. Du kan også kontrollere status for agenten i Azure-portalen ved at klikke på knappen Vis lokale agenter.
3. Sørg for, at du angiver værdien for feltet "Brugernavn på arbejdsdag" ved hjælp username@workday formatet -lejer-navn. Hvis navnet på arbejdsdagen-lejeren mangler, mislykkes godkendelse af Arbejdsdag.
4. Hvis du konfigurerer integrationen med implementeringslejeren for Arbejdsdag, skal du notere den planlagte nedetid for din arbejdsdag-lejer. Arbejdsdagen har planlagt nedetid for dens implementeringslejere over weekender (som regel fra fredag aften til lørdag morgen), og forbindelsesfejl i denne nedetidsperiode er et kendt problem, der løses automatisk, så snart implementeringslejerne igen er online.
5. I sjældne tilfælde får du muligvis også vist denne fejl, hvis adgangskoden til integrationssystembrugeren ændres på grund af lejeropdatering, eller hvis kontoen er i låst eller udløbet tilstand. Kontrollér status for integrationssystembrugeren med arbejdsdagsadministratoren.

Du kan finde flere oplysninger om konfiguration af arbejdsdagen for automatisk klargøring i [Selvstudium: Konfigurer arbejdsdag til automatisk bruger klargøring](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
