---
title: Problemer med tokens
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916737"
---
# <a name="issues-with-tokens"></a>Problemer med tokens

Hvis du vil administrere problemer, der er relateret til tokens, kan du udføre følgende trin:

1. Du kan angive levetiden for en Access-, ID-eller SAML-token, der er udstedt af Microsoft Identity platform. Du kan angive levetiden for tokens for alle apps i organisationen, for et program med flere arkitekturer (flere virksomheder) eller for en bestemt tjeneste Principal i organisationen. Hvis du vil have mere at vide, skal du se [levetiden for konfigurerbare tokens i Microsoft Identity platform (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Access-tokens gør det muligt for klienter at ringe til beskyttede API'er på internettet og bruges af webapi'erne til at udføre godkendelse og godkendelse. Som det er en OAuth-specifikation, er Access-tokens ugennemsigtige strenge uden et angivet format – visse identitetsudbydere (IDPs) bruger GUID'ER, andre bruger krypterede blob. Microsoft Identity platform bruger en række forskellige Access-tokens, afhængigt af konfigurationen af API'ET, der accepterer tokenet. Du kan få mere at vide om, hvordan din API kan validere og bruge kravene i et adgangstoken, under [adgangs tokens til Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Microsoft-godkendelses biblioteket (MSAL) understøtter flere godkendelses strømme til brug i forskellige programscenarier. Du kan få mere at vide under [godkendelses strømme](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. OAuth 2,0-godkendelseskode-Grant kan bruges i apps, der er installeret på en enhed for at få adgang til beskyttede ressourcer, f. eks. webapi'er. Ved hjælp af Microsoft Identity platform implementation of OAuth 2,0, kan du tilføje logon-og API-adgang til dine mobile-og skrivebordsprogrammer. Se [Microsoft Identity platform og OAuth 2,0 Authorization-kode flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) for at finde ud af, hvordan du bruger programmet direkte mod protokollen i dit program, ved hjælp af et hvilket som helst sprog.
5. OpenID Connect (OIDC) er en godkendelsesprotokol, der er bygget på OAuth 2,0, som du kan bruge til at logge på et sikkert program for en bruger. Når du bruger Microsoft Identity platform-slutpunktets implementering af OpenID Connect, kan du tilføje logon-og API-adgang til dine apps. [Microsoft Identity platform og OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) viser, hvordan du gør dette uafhængigt af sprog og beskriver, hvordan du sender og modtager http-meddelelser uden at bruge Microsoft open-source-biblioteker.
    - UserInfo-slutpunktet er en del af OIDC-standarden, der er beregnet til at returnere krav om brugeren, der er godkendt. Du kan finde flere oplysninger i [Microsoft Identity platform UserInfo Endpoint](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Når du [ringer til en webapi i en Web App ved hjælp af Azure ad og OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) -eksemplet, viser det, hvordan du opretter et MVC-webprogram, der bruger Azure ad til logon ved hjælp af protokollen OpenID Connect, og derefter kalder en webapi under den identitet, der er logget på, ved hjælp af tokens, der er opnået via OAuth 2,0. I dette eksempel bruges OpenID Connect ASP .net OWIN-middleware and ADAL .net.
6. [Konfigurere et program for at få vist en webapi](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -i denne hurtigstarter skal du registrere et webapi med Microsoft Identity platform og vise det til klientprogrammer ved at tilføje et eksempelområde. Ved at registrere dit Web-API og afsløre det via omfang, kan du give tilladelses baseret adgang til ressourcerne til autoriserede brugere og klientprogrammer, der har adgang til din API.
7. I Azure Active Directory B2C (Azure AD B2C) er flowet for ressource ejeradgangskoden (ROPC) et OAuth-standard flow for standardgodkendelse. I dette flow udveksler et program, også kaldet den afhængige part, nogle gyldige legitimationsoplysninger for tokens. Legitimationsoplysningerne omfatter et bruger-ID og en adgangskode. De tokens, der returneres, er et ID-token, et adgangstoken og et opdaterings token. Hvis du vil have mere at vide, skal du se [konfigurere en adgangskode for legitimationsoplysninger for ressource ejer i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

