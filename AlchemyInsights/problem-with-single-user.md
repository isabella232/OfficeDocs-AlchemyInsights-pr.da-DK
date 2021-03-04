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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429468"
---
# <a name="problem-with-single-user"></a>Problem med enkelt bruger

- Brugeren er muligvis ikke blevet klargjort, fordi tjenesten endnu ikke har haft mulighed for at evaluere brugeren. Gennemgå vejledningen for, hvor lang tid klargøring tager, samt statuslinjen på konfigurationssiden for klargøring. Hvis den konstante tilstand, der er angivet i sektionen med yderligere oplysninger, er før den dato, hvor brugeren blev oprettet/opdateret/slettet, betyder det, at vi endnu ikke har evalueret brugeren. I dette scenarie er det bedste at vente på, at klargøringstjenesten afsluttes.

  - Bemærk, at vores tjeneste kun er opmærksom på ændringer for en bruger i kildesystemet (Cloud HR). Der skal være en gyldig ændring i kildesystemet for Azure AD for at registrere ændringen og få den til at flyde ind i Active Directory.
- Klargøringstjenesten evaluerede brugeren og vurderede, at den ikke skulle klargøres:
  - Hvis du har angivet en attribut baseret på et filter til angivelse af område, skal du sikre dig, at brugeren opfylder de kriterier, du har angivet.
  - Hvis brugerne allerede findes i destinationssystemet og brugerens tilstand i kilde- og målmatchet, vil vi ikke gøre yderligere.
- Klargøringstjenesten forsøgte at klargøre brugeren, og det mislykkedes. For disse scenarier skal du gennemgå fanen med fejlfinding og anbefalinger i klargøringslogfilerne:
  - En påkrævet attribut for brugeren mangler muligvis i Active Directory i det lokale miljø eller Azure AD. For eksempel genererer userPrincipalName- eller sAMAccountName-regler ikke den rigtige værdi.
  - Den matchende attribut (som regel medarbejder-id) løses ikke til en entydig bruger i Active Directory i det lokale miljø eller Azure AD. Der er f.eks. to brugere med det samme medarbejder-id i AD, og tjenesten returnerer en fejlkode, der angiver dublerede målposter for den samme kildepost.

Se klargøringslogfilerne for et problem med en bestemt bruger, hvis du vil gennemse [logfiler for enkeltbrugere](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)og grupper.
