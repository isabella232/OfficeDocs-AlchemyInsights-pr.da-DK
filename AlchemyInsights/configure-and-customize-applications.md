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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044982"
---
# <a name="configure-and-customize-applications"></a>Konfigurere og tilpasse programmer

**Konfigurer programmer**

1. [Hurtig start: Konfigurer egenskaberne for](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) et program i din Azure Active Directory (Azure AD)-lejer viser, hvordan du konfigurerer nogle af egenskaberne for en app.
2. For at integrere dine programmer med Azure Active Directory har vi udviklet en [samling selvstudier, der](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) hjælper dig gennem konfigurationen.
3. [Sådan konfigurerer du et](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) programproxyprogram hjælper dig med at forstå, hvordan du konfigurerer et programproxyprogram i Azure AD, så dine programmer i det lokale miljø vises i skyen.
4. [Download PingAccess,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)og konfigurer dit program: Følg instruktionerne i Konfigurer *PingAccess til Azure AD for* at beskytte programmer, der er udgivet ved hjælp af Microsoft Azure AD-programproxy på pingidentitetswebstedet, og download den nyeste version af PingAccess.

**Fejl i et forkert konfigureret program (AADSTS650056)**

1. Sørg for, at du tilgår programmet fra den logonadresse, du har angivet af programejeren. Ellers skal du logge på programmet via dets normale proces. I de fleste tilfælde løses problemet automatisk på en naturlig måde. Hvis det ikke sker, kan dette indlæg hjælpe med at foretage fejlfinding og løse problemet.
2. **Hvis din organisation ejer programmet (hvilket** betyder, at programregistreringen er i din organisation):
    - Vi anbefaler som minimum, at `User.Read` den eller delegerede tilladelse fra Microsoft `openid` **Graph** tilføjes.
    - Sørg for, at programmet og alle dets tilladelser er accepteret. Det kan du kontrollere ved at se på **kolonnen Status** i Programregistrering i **API-tilladelser.**
    - I visse situationer kan programmet være tredjepart, men det kan være registreret i din organisation. Bekræft, om dette program er angivet i dine App-registreringer (ikke Enterprise-programmer).
    - Hvis du fortsat får vist denne fejlmeddelelse. Derefter skal du muligvis oprette den URL-adresse til samtykke, som blev beskrevet **i trin 4.**
3. **Hvis din organisation ikke er programejer og bruger det som et tredjepartsprogram:**
    - Hvis du er global/firmaadministrator, bør du kunne se samtykkeskærmen. Sørg for at markere afkrydsningsfeltet **"Samtykke på vegne af din organisation".**
    - Hvis du ikke kan se skærmbilledet med samtykke, skal du slette virksomhedsprogrammet og prøve igen.
    - Hvis du fortsat får vist denne fejlmeddelelse. Derefter skal du muligvis oprette den URL-adresse til samtykke, som blev beskrevet **i trin 4.**
4. **Opret samtykke-URL-adressen** manuelt, så den kan bruges: Hvis programmet er udviklet til at få adgang til en bestemt ressource, kan du muligvis ikke bruge knapperne Samtykke fra Azure-portalen, skal du oprette din egen URL-adresse til samtykke manuelt og bruge denne.
    - Du skal hente og `{App-Id}` hente fra `{App-Uri-Id}` programejeren. `{Tenant-Id}` være dit lejer-id. Dette vil enten være eller `yourdomain.onmicrosoft.com` dit katalog-id.
    - Hvis programmet tilgår sig selv for ressourcen, vil `{App-Id}` og `{App-Uri-Id}` være det samme.
5. Du kan få mere at vide [under Problemer med at logge på SAML-baserede enkelt sign-on-konfigurerede apps.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Tilpas programmer**

- Føj branding til din organisations [Azure Active Directory-logonside](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) – Brug organisationens logo og brugerdefinerede farveskemaer for at give dine Azure Active Directory-logonsider (Azure AD) et ensartet udseende.
- [Tilføj dit brugerdefinerede domænenavn ved hjælp Azure Active Directory -Alle](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) nye Azure AD-lejere har et indledende domænenavn. Du kan ikke ændre eller slette det oprindelige domænenavn, men du kan tilføje organisationens navne. Tilføjelse af brugerdefinerede domænenavne hjælper dig med at oprette brugernavne, der er velkendte for dine brugere.
