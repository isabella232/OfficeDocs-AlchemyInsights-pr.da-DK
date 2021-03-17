---
title: Konfigurer Seamless Single Sign-on (SSO)
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
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841460"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurer Seamless Single Sign-on (SSO)

**Konfigurere programmer**

1. Du skal hente værdierne fra programleverandøren. Du kan manuelt angive værdierne eller overføre en metadatafil for at udtrække værdien af felterne.
2. Mange apps er allerede konfigureret på forhånd til at fungere sammen med Azure AD. Disse apps vises i galleriet med apps, som du kan gennemse, når du føjer en app til din Azure AD-lejer. [Hurtigstarter-serien](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) gennemgår processen.
3. Hvis du vil oprette et program, som ikke er et galleri, kan du klikke på **+ Opret** din egen programknap og give dit program et navn.
    - Som standard vælger den **Integrer** alle andre programmer, du ikke finder i galleriet, hvilket er den korrekte indstilling for ikke-galleriprogrammer.
    - Når du trykker **på Opret,** efter du har oprettet navnet på programmet, oprettes et nyt Enterprise-program, som ikke er galleriet.
    - Derefter kan du navigere til **Enkelt logon** under **Administrer** af det pågældende program, og du vil kunne se forskellige teknikker til implementering af det i dit miljø.

**Konfigurere problemfri SSO for et bestemt program**

Til appsene i galleriet finder du detaljerede, trinvise instruktioner. Du kan få adgang til trinnene ved at gennemse en liste over alle selvstudier til appkonfiguration på [SaaS-selvstudier til appkonfiguration.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurere SAML-baseret SSO**

1. [Hurtig start: Konfigurer SAML-baseret enkelt-logon (SSO) for et program i din Azure Active Directory (Azure AD)-lejer.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Hvis du vil have mere at vide om SAML-baseret indstilling for enkelt-logon, skal du se [Forstå SAML-baseret enkelt-logon.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Du kan få mere at vide om SAML 2.0-godkendelsesanmodninger og svar, som Azure Active Directory (Azure AD) understøtter til Enkelt Sign-On (SSO), under [Single Sign-On SAML-protokollen.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Hvis du vil have mere at vide om, hvordan du opretter og konfigurerer et SAML-baseret enkelt-logon (SSO) til dit program i Azure Active Directory (Azure AD) ved hjælp af Microsoft Graph API, skal du se [Konfigurere SAML-baseret enkelt-logon til](https://docs.microsoft.com/graph/application-saml-sso-configure-api)dit program ved hjælp af Microsoft Graph API.
5. Hvis du vil vide, hvordan Azure AD bruger SAML-protokollen, skal du se, [hvordan Microsoft-identitetsplatformen bruger SAML-protokollen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfigurere tokens og krav**

1. [Sådan gør du: Tilpas krav udstedt i SAML-token til virksomhedsprogrammer.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Hvis du vil lære, hvordan du konfigurerer krav ved hjælp af PowerShell, skal du se Sådan gør du: Tilpas krav, der sendes i tokens for en bestemt app i en lejer [(forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Du kan få mere at vide om, hvordan du konfigurerer valgfrie krav, under Sådan gør du: Angiv [valgfrie krav til din app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Hvis du vil lære at bruge attributter for katalogskemaudvidelse til at sende brugerdata til programmer i token-krav, skal du se Brug af udvidelsesattributter til [mappeskema i krav.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Du kan få mere at vide om, hvordan du konfigurerer tokenlevetiderne, under [Konfigurerbar tokenlevetid på Microsoft-identitetsplatformen (prøveversion).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurer politikker for tokens levetid (forhåndsvisning)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – I denne artikel gennemgår vi et fælles politikscenarie, der kan hjælpe dig med at indføre nye regler for tokenlevetid. I eksemplet lærer du, hvordan du opretter en politik, der kræver, at brugere godkender oftere i din webapp.

**Fejlfinding af SSO-konfiguration**

- For ofte stillede spørgsmål om Azure Active Directory Seamless Single Sign-On (Seamless SSO) skal du se [Azure Active Directory Seamless Single Sign-On: Ofte stillede spørgsmål.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Hvis du vil have oplysninger om fejlfinding af almindelige problemer med Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), skal du se Fejlfinding [af Azure Active Directory Seamless Single Sign-On.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
