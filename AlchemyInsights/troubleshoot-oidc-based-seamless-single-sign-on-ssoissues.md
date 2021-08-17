---
title: Fejlfinding af OIDC-baserede problemer med enkelt logon (Seamless Single Sign-on)
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
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105764"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Fejlfinding af OIDC-baserede problemer med enkelt logon (Seamless Single Sign-on)

- Hvis du vil have mere at vide om, hvordan du føjer en OIDC-baseret app til din Azure-lejer, skal du se Hurtig start: Konfigurer [OIDC-baseret SSO (single sign-on) til](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)et program i din Azure Active Directory-lejer (Azure AD).
- Hvis du vil have mere at vide om apps, der bruger OpenID Forbind-standarden til at implementere enkelt logon, skal du se [Forstå OIDC-baseret enkelttegn på](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Hvis du vil have mere at vide, hvis du vælger at skrive din kode direkte ved at sende og håndtere HTTP-anmodninger eller bruge et open source-bibliotek fra en tredjepart i stedet for at bruge et af vores open source-biblioteker, skal du se [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)og OpenID Forbind-protokollerne på Microsoft-identitetsplatform.

**Protokoller**

1. [Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) og implicit tildelingsflow – Den definerende egenskab ved den implicitte tildeling er, at tokens (id-tokens eller adgangstokens) returneres direkte fra /authorize-slutpunktet i stedet for /token-slutpunktet. Dette bruges ofte som en del af godkendelseskodeflowet, i det der kaldes **"hybridflow"**- henter id-token på /authorize-anmodningen sammen med en godkendelseskode. I denne artikel beskrives det, hvordan du programmerer direkte mod protokollen i dit program for at anmode om tokens fra Azure AD.
2. Microsoft-identitetsplatform og [OAuth 2.0-godkendelseskodeflow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Godkendelseskoden OAuth 2.0 kan bruges i apps, der er installeret på en enhed, til at få adgang til beskyttede ressourcer, f.eks web-API'er. Ved Microsoft-identitetsplatform implementering af OAuth 2.0 kan du tilføje logon og API-adgang til dine **mobil- og skrivebordsapps.** I denne artikel beskrives det, hvordan du programmerer direkte mod protokollen i dit program på et hvilket som helst sprog.
3. Microsoft-identitetsplatform og [OpenID Forbind-protokollen](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Når du bruger Microsoft-identitetsplatform's implementering af OpenID-Forbind, kan du tilføje logon- og API-adgang til dine apps. I denne artikel beskrives det, hvordan du gør dette uafhængigt af sproget, og det beskrives, hvordan du kan sende og modtage HTTP-meddelelser uden brug af **Microsoft Open Source-biblioteker.**
4. Microsoft-identitetsplatform og flowet til klientlegitimationsoplysninger for [OAuth 2.0- og OAuth 2.0-klienten,](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) der er angivet i RFC 6749, nogle gange kaldet **to-legged OAuth,** til at få adgang til webbaserede ressourcer ved hjælp af identiteten af et program. Denne type tildeling bruges ofte til server til server-interaktioner, der skal køre i baggrunden, uden øjeblikkelig interaktion med en bruger. Disse typer programmer kaldes ofte **for daemoner eller** **tjenestekonti.** I denne artikel beskrives det, hvordan du programmerer direkte mod protokollen i programmet.
