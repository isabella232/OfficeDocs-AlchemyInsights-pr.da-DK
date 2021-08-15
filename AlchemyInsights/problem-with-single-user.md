---
title: Problem med enkelt bruger
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
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960145"
---
# <a name="problem-with-single-user"></a>Problem med enkelt bruger

- Brugeren er muligvis ikke blevet klargjort, fordi tjenesten ikke har haft mulighed for at evaluere brugeren endnu. Gennemgå vejledningen for, hvor lang tid klargøring tager, samt statuslinjen på siden konfiguration af klargøring. Hvis den stille tilstand, der er angivet i sektionen med yderligere oplysninger, er før den dato, hvor brugeren blev oprettet/opdateret/slettet, betyder det, at vi endnu ikke har evalueret brugeren. I dette scenarie er det bedste at vente på, at klargøringstjenesten afsluttes.

  - Bemærk, at vores tjeneste kun er opmærksom på ændringer af en bruger i kildesystemet (Cloud HR). Der skal være en gyldig ændring i kildesystemet til Azure AD for at registrere ændringen og få den til at flyde ind i Active Directory.
- Klargøringstjenesten evaluerede brugeren og vurderede, at den ikke skulle klargøres:
  - Hvis du har angivet et attributbaseret områdefilter, skal du sikre dig, at brugeren opfylder de kriterier, du har angivet.
  - Hvis brugerne allerede findes i destinationssystemet og brugerens tilstand i kilde- og målmatchet, vil vi ikke gøre yderligere.
- Klargøringstjenesten forsøgte at klargøre brugeren, og den mislykkedes. For disse scenarier skal du gennemgå fanen til fejlfinding og anbefalinger i klargøringslogfilerne:
  - En påkrævet attribut på brugeren mangler muligvis i Active Directory eller Azure AD i det lokale miljø. Eksempelvis genererer userPrincipalName- eller sAMAccountName-generationsregler ikke den rigtige værdi.
  - Den matchende attribut (som regel medarbejder-id) løses ikke til en entydig bruger i Active Directory eller Azure AD i det lokale miljø. Der er f.eks. to brugere med det samme medarbejder-id i AD, og tjenesten returnerer en fejlkode, der angiver dublerede målposter for den samme kildepost.

Hvis du vil gennemse logfiler for enkeltbrugere og grupper, skal du se Gennemse [klargøringslogfilerne for et problem med en bestemt bruger.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
