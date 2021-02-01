---
title: Konfigurere og tilpasse programmer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063594"
---
# <a name="configure-and-customize-applications"></a>Konfigurere og tilpasse programmer

**Konfigurere programmer**

1. Hurtig start: Konfigurer egenskaberne for et program i din [Azure Active Directory-lejer (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) viser, hvordan du konfigurerer nogle af egenskaberne for en app.
2. For at integrere dine programmer med Azure Active Directory har vi udviklet en [samling af selvstudier,](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) der hjælper dig gennem konfigurationen.
3. [Sådan konfigurerer du et](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) programproxyprogram, der hjælper dig med at forstå, hvordan du konfigurerer et programproxyprogram i Azure AD, så dine lokale programmer vises i skyen.
4. [Download PingAccess,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)og konfigurer dit program: Følg instruktionerne i *Configure PingAccess for Azure AD for* at beskytte programmer, der er udgivet ved hjælp af Microsoft Azure AD Application Proxy på webstedet Ping Identity, og download den nyeste version af PingAccess.

**Fejlkonfigureret program (AADSTS650056)**

1. Sørg for, at du tilgår programmet fra den logonadresse, du har angivet af programejeren. Ellers skal du logge på programmet via dets normale proces. I de fleste tilfælde løses problemet automatisk naturligt. Hvis det ikke sker, kan dette indlæg hjælpe med at foretage fejlfinding og løse problemet.
2. **Hvis din organisation ejer programmet (dvs.** at programregistreringen er i din organisation):
    - Vi anbefaler som minimum, at `User.Read` den eller de delegerede tilladelser fra Microsoft `openid` **Graph** tilføjes.
    - Sørg for, at programmet og alle dets tilladelser er accepteret. Du kan kontrollere dette  ved at se på statuskolonnen i programregistreringen i **API-tilladelser.**
    - I visse situationer kan programmet være en tredjepart, men det kan være registreret i din organisation. Bekræft, om dette program er angivet i dine appregistreringer (Ikke Enterprise-programmer).
    - Hvis du fortsat får vist denne fejlmeddelelse. Derefter skal du muligvis oprette den URL-adresse til samtykke, der er beskrevet **i trin 4.**
3. **Hvis din organisation ikke er programejer og bruger den som et tredjepartsprogram:**
    - Hvis du er global/firmaadministrator, bør du se skærmbilledet med samtykke. Sørg for at markere afkrydsningsfeltet **"Samtykke på vegne af din organisation".**
    - Hvis du ikke kan se samtykkeskærmen, skal du slette Enterprise-programmet og prøve igen.
    - Hvis du fortsat får vist denne fejlmeddelelse. Derefter skal du muligvis oprette den URL-adresse til samtykke, der er beskrevet **i trin 4.**
4. **Opbyg** url-adressen til samtykke manuelt, så den kan bruges: Hvis programmet er udviklet til at få adgang til en bestemt ressource, kan du muligvis ikke bruge samtykkeknapperne fra Azure-portalen, du skal oprette din egen URL-adresse til samtykke manuelt og bruge denne.
    - Du skal hente og `{App-Id}` fra `{App-Uri-Id}` programejeren. `{Tenant-Id}` være dit lejer-id. Dette er enten dit `yourdomain.onmicrosoft.com` mappe-id.
    - Hvis programmet tilgår sig selv for ressourcen, vil `{App-Id}` det være det samme og det `{App-Uri-Id}` samme.
5. Du kan få mere at vide [under Problemer med at logge på SAML-baserede apps, der er konfigureret til enkelt logon.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Tilpas programmer**

- Føj branding til din organisations [logonside til Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – Brug organisationens logo og brugerdefinerede farveskemaer for at give dine logonsider i Azure Active Directory (Azure AD) et ensartet udseende.
- [Tilføj dit brugerdefinerede domænenavn ved hjælp af Azure Active Directory-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – Hver ny Azure AD-lejer har et indledende domænenavn. Du kan ikke ændre eller slette det indledende domænenavn, men du kan tilføje organisationens navne. Tilføjelse af brugerdefinerede domænenavne hjælper dig med at oprette brugernavne, der er velkendte for dine brugere.
