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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481852"
---
# <a name="configuring-the-provision-service"></a>Konfiguration af klargøringstjenesten

For at automatisere klargøring af brugere kan fungere, kræver Azure AD gyldige legitimationsoplysninger, der giver mulighed for at oprette forbindelse til ARBEJDSDAG Web Services API. Desuden validerer knappen Testforbindelse på appen Arbejdsdag til AD-bruger klargøring også, om den kan oprette forbindelse til den Azure AD Connect-klargøringsagent, der er knyttet til AD-domænet.

Hvis Azure-portalen returnerer en fejl, når du gemmer legitimationsoplysningerne, skal du følge de anbefalede trin nedenfor:

1. Bekræft, at du har konfigureret arbejdsdagens integrationssystembrugerkonto som nævnt i selvstudiet om konfiguration [af integrationssystembruger i Arbejdsdag.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Bekræft, at Azure AD Connect Provisioning Agent Service er oppe at køre på din lokale Windows-server ved hjælp af Services Management Console. Du kan også kontrollere status for agenten i Azure-portalen ved at klikke på knappen Vis lokale agenter.
3. Sørg for, at du angiver værdien for feltet "Arbejdsdagens brugernavn" ved hjælp username@workday-lejer-navn. Hvis navnet på arbejdsdag-lejeren mangler, mislykkes godkendelse af arbejdsdagen.
4. Hvis du konfigurerer integrationen med implementeringslejeren for Arbejdsdag, skal du notere de planlagte nedetidstimer for din arbejdsdags lejer. Arbejdsdagen har planlagt nedetid for dens implementeringslejere over weekender (som regel fra fredag aften til lørdag morgen), og forbindelsesfejl i denne nedetidsperiode er et kendt problem, der løses automatisk, så snart implementeringslejerne igen er online.
5. I sjældne tilfælde får du muligvis også vist denne fejl, hvis adgangskoden til systembrugeren til integration ændres på grund af lejeropdatering, eller hvis kontoen er i låst eller udløbet tilstand. Kontrollér status for integrationssystembrugeren med din arbejdsdagsadministrator.

Du kan finde flere oplysninger om konfiguration af arbejdsdagen for automatisk klargøring i [Selvstudium: Konfigurer arbejdsdag til automatisk klargøring af brugere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
