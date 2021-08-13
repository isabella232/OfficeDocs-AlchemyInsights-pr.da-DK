---
title: Bruger klargøring
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971333"
---
# <a name="user-provisioning"></a>Bruger klargøring

- Brug [klargøringsfunktionaliteten efter](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) behov til at klargøre en bruger og få detaljeret diagnosticering af de trin, der er taget.
- Hvis du vil foretage fejlfinding af problemer, der opstår under klargøring af brugere og grupper, skal du se [fejlfindingsvejledningen Ingen brugere klargøres.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Hvis du bemærker, at brugerne ikke bliver klargjort, kan du se [Klargøringslogfiler (preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) Azure Active Directory (AD). Søg efter logposter, der er relevante for en bestemt bruger.
- Genstart med jævne mellemrum klargøring for at fange eventuelle brugere, der er blevet overset i en tidligere klargøringscyklus.
- Brugeren/gruppen er muligvis ikke blevet klargjort, fordi vores tjeneste endnu ikke har haft mulighed for at evaluere brugeren. Gennemgå vejledningen for, hvor lang tid klargøring tager, samt statuslinjen på siden konfiguration af klargøring. Hvis den stille tilstand, der er angivet i sektionen med yderligere oplysninger, er før den dato, hvor brugeren blev oprettet/opdateret/slettet, betyder det, at vi endnu ikke har evalueret brugeren. I dette scenarie er det bedste at vente på, at klargøringstjenesten afsluttes. Hvis du har opnået en stabil tilstand, anbefaler vi, at du udfører en genstart fra brugergrænsefladen i Azure-portalen.
  - Bemærk, at vores tjeneste kun er opmærksom på ændringer af en bruger/gruppe i kildesystemet (Azure Active Directory). Hvis en bruger/gruppe fjernes direkte i programmet (f.eks. ServiceNow), er vi ikke opmærksomme på disse ændringer og kan ikke rulle den tilbage baseret på brugerens tilstand i kildesystemet. I dette scenarie er det bedst at tilbagerulle ændringen direkte i destinationsprogrammet.
- Vores tjeneste evaluerede brugeren/gruppen og vurderede, at den ikke skulle klargøres:
  - Hvis du har indstillet området til tildelte brugere og grupper, skal du kontrollere, om brugeren/gruppen er tildelt til programmet.
  - Hvis brugeren/gruppen er tildelt til programmet, skal du sikre dig, at de ikke er tildelt standardadgangsrollen. Denne rolle kan ikke bruges til klargøring.
  - Hvis du har angivet et attributbaseret områdefilter, skal du sikre dig, at brugeren opfylder de kriterier, du har angivet.
  - Hvis brugerne allerede findes i destinationssystemet og brugerens tilstand i kilde- og målmatchet, vil vi ikke gøre yderligere.
- Vores tjeneste forsøgte at klargøre brugeren, og det mislykkedes. For disse scenarier skal du gennemgå fanen til fejlfinding og anbefalinger i klargøringslogfilerne:
  - En påkrævet attribut på brugeren mangler muligvis i Azure Active Directory eller svarer ikke til det format, der kræves af tredjepartsprogrammet. Eksempelvis kan attributten Land for en bruger være indstillet til USA, når den skal være USA.
  - Attributten er en referentiel attribut, der endnu ikke findes i destinationsprogrammet. En referentiel attribut er en attribut, der peger på et andet objekt, f.eks. en bruger, der er medlem af en gruppe. Brugerens id vil være i medlemsattributten for gruppen, men det kan kun behandles, hvis det brugerobjekt, det peger på, allerede findes.
