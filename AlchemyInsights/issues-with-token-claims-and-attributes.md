---
title: Problemer med tokenkrav og attributter
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035853"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemer med tokenkrav og attributter

**Opdater, konfigurer eller fjern token-krav**

1. Ved hjælp af Azure Active Directory (Azure AD) kan du tilpasse kravtypen [for](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) rollekravet i det svartoken, du modtager, når du godkender en app.
2. Programudviklere kan bruge valgfrie krav i deres Azure AD-programmer til at angive, hvilke krav de ønsker i tokens, der sendes til deres program. Du kan finde flere oplysninger [i Angiv valgfrie krav til din app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurere gruppekrav for programmer med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. Hvis du bruger Seamless Single Sign-on i dit program, skal du se tilpassede krav, [der er udstedt i SAML-tokenet til virksomhedsprogrammer.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Tilknytning af kravattribut**

1. Hvis du vil konfigurere politikken for tilknytning af krav ved hjælp af PowerShell, skal du se Tilpasse krav, der er blevet udsendt i tokens for en bestemt app i [en lejer (forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Udvidelsesattributter til katalogskemaer gør det muligt at gemme yderligere data i Azure Active Directory på brugerobjekter og andre katalogobjekter, f.eks. grupper, lejeroplysninger, tjeneste principaler. Kun udvidelsesattributter på brugerobjekter kan bruges til at udsende krav til programmer. [Brug af attributter for katalogskemaudvidelser](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) i krav beskriver, hvordan du bruger attributter for katalogskemaudvidelse til at sende brugerdata til programmer i token-krav.

Du kan finde flere oplysninger om token-krav i:

- [Krav i adgangstokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Krav i en id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Krav, som](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) du kan forvente i id-tokens og adgangstokens udstedt af Azure AD B2C
- [Saml token-kravreference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
