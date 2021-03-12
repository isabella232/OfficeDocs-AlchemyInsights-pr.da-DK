---
title: Fejlfinding af problemer med OIDC-baseret SSO (Seamless Single Sign-on)
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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743972"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Fejlfinding af problemer med OIDC-baseret SSO (Seamless Single Sign-on)

- Hvis du vil lære, hvordan du føjer en OIDC-baseret app til din Azure-lejer, skal du se Hurtig start: Konfigurer OIDC-baseret enkelt logon (SSO) for et program i din [Azure Active Directory-lejer (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Hvis du vil have mere at vide om apps, der bruger OpenID Connect-standarden til at implementere enkelt-logon, skal du se [Forstå OIDC-baseret enkelt-logon.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Hvis du vil have mere at vide, hvis du vælger at skrive din kode ved direkte at sende og håndtere HTTP-anmodninger eller bruge et open source-bibliotek fra en tredjepart i stedet for at bruge et af vores open source-biblioteker, skal du se [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)og OpenID Connect-protokollerne på Microsoft-identitetsplatformen.

**Protokoller**

1. [Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) og implicit tildelingsflow – Den definerende egenskab ved den implicitte tildeling er, at tokens (id-tokens eller adgangstokens) returneres direkte fra /authorize-slutpunktet i stedet for /token-slutpunktet. Dette bruges ofte som en del af godkendelseskodeflowet i det, der kaldes **"hybridflowet"**– henter id-tokenet på /authorize-anmodningen sammen med en godkendelseskode. I denne artikel beskrives det, hvordan du programmerer direkte mod protokollen i dit program for at anmode om tokens fra Azure AD.
2. Microsoft-identitetsplatform og [OAuth 2.0-godkendelseskodeflow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Godkendelseskoden OAuth 2.0 kan bruges i apps, der er installeret på en enhed, for at få adgang til beskyttede ressourcer, f.eks web-API'er. Ved hjælp af Microsoft-identitetsplatformens implementering af OAuth 2.0 kan du tilføje logon og API-adgang til dine **mobil- og skrivebordsapps.** Denne artikel beskriver, hvordan du programmerer direkte mod protokollen i dit program ved hjælp af et hvilket som helst sprog.
3. [Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) og OpenID Connect-protokollen – Når du bruger Microsoft-identitetsplatformens implementering af OpenID Connect, kan du tilføje logon- og API-adgang til dine apps. I denne artikel beskrives det, hvordan du gør dette uafhængigt af sproget, og det beskrives, hvordan du sender og modtager HTTP-meddelelser uden at bruge **Microsoft Open Source-biblioteker.**
4. [Microsoft-identitetsplatform og flowet til OAuth 2.0-klientlegitimationsoplysninger](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Du kan bruge OAuth 2.0-klientlegitimationsoplysninger, der er angivet i RFC 6749, nogle gange kaldet tobenede **OAuth,** til at få adgang til webbaserede ressourcer ved hjælp af identiteten af et program. Denne type tildeling bruges ofte til server-til-server-interaktioner, der skal køre i baggrunden uden øjeblikkelig interaktion med en bruger. Disse typer af programmer kaldes ofte **daemoner eller** **tjenestekonti.** I denne artikel beskrives det, hvordan du programmerer direkte mod protokollen i dit program.
