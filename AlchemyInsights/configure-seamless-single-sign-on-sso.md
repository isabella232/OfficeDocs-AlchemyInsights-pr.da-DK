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
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966031"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurer Seamless Single Sign-on (SSO)

**Konfigurer programmer**

1. Du skal hente værdierne fra programleverandøren. Du kan indtaste værdierne manuelt eller overføre en metadatafil for at udtrække værdien af felterne.
2. Mange apps er allerede konfigureret på forhånd til at fungere sammen med Azure AD. Disse apps vises i galleriet med apps, som du kan gennemse, når du føjer en app til din Azure AD-lejer. [Hurtigstarter-serien](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) gennemgår processen.
3. Hvis du vil oprette et program, der ikke er et galleri, kan du klikke på **+** Opret din egen programknap og give dit program et navn.
    - Som standard vælger den **Integrer ethvert** andet program, du ikke finder i galleriet, som er den korrekte indstilling for ikke-galleriprogrammer.
    - Når du trykker **på Opret,** efter at du har oprettet navnet på programmet, oprettes der et nyt Virksomhedsprogram, som ikke er galleriet.
    - Derefter kan du gå til **Enkelt** logon **under** Administrer af det pågældende program, og du vil kunne se forskellige teknikker til implementering af det i dit miljø.

**Konfigurere Seamless SSO til et bestemt program**

Til appsene i galleriet finder du detaljerede, trinvise instruktioner. For at få adgang til trinnene kan du gennemse en liste over alle selvstudier til appkonfiguration [på SaaS-selvstudier til appkonfiguration](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Konfigurere SAML-baseret SSO**

1. [Hurtig start: Konfigurer SAML-baseret enkelt logon (SSO) for](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)et program i din Azure Active Directory (Azure AD).
2. Hvis du vil have mere at vide om SAML-baseret indstilling for enkelt logon, skal du se [Forstå SAML-baseret enkelttegn på](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Du kan få mere at vide om SAML 2.0-godkendelsesanmodninger og -svar, som Azure Active Directory (Azure AD) understøtter til enkeltstående Sign-On (SSO) i Single [Sign-On SAML-protokollen.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Du kan få mere at vide om, hvordan du opretter og konfigurerer en SAML-baseret enkelt logon (SSO) til dit program i Azure Active Directory (Azure AD) ved hjælp af Microsoft Graph API under [Konfigurer SAML-baseret enkelttegn til](https://docs.microsoft.com/graph/application-saml-sso-configure-api)dit program ved hjælp af Microsoft Graph API.
5. Du kan få mere at vide om, hvordan Azure AD bruger [SAML-protokollen, under Sådan Microsoft-identitetsplatform SAML-protokollen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfigurer tokens og krav**

1. [Sådan gør du: Tilpas krav, der er udstedt i SAML-token til virksomhedsprogrammer.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Du kan få mere at vide om, hvordan du konfigurerer krav ved hjælp af PowerShell under Sådan gør du: Tilpas krav, der er blevet sendt i tokens for en bestemt app i en lejer [(forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Du kan få mere at vide om, hvordan du konfigurerer [valgfrie krav, under Sådan gør du: Angiv valgfrie krav til din app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Hvis du vil lære, hvordan du bruger udvidelsesattributter for katalogskemaer til at sende brugerdata til programmer i token-krav, skal du se Brug af attributter til [katalogskemaudvidelse i krav](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Du kan få mere at vide om, hvordan du konfigurerer tokenlevetiderne, under Konfigurerbar tokenlevetid [i Microsoft-identitetsplatform (forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurer politikker for tokenlevetid (forhåndsvisning)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – I denne artikel gennemgår vi et fælles politikscenarie, der kan hjælpe dig med at opstille nye regler for tokenlevetid. I eksemplet lærer du, hvordan du opretter en politik, der kræver, at brugere godkendes oftere i din webapp.

**Fejlfinding af SSO-konfiguration**

- For ofte stillede spørgsmål om Azure Active Directory Seamless Single Sign-On (Seamless SSO) skal [du Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Du kan finde fejlfindingsoplysninger om almindelige problemer med Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO) i [Fejlfinding Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
