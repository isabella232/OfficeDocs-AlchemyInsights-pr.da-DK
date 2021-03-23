---
title: Fejlfinding af protokollerne OAuth 2.0 og OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035598"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Fejlfinding af protokollerne OAuth 2.0 og OpenID Connect

Du kan løse problemer med OAuth 2.0 og OpenID Connect ved at udføre følgende anbefalede trin:

Se følgende artikler, der er relateret til konfiguration og fejlfinding af protokollerne OAuth 2.0 og OpenID Connect:

- Microsoft-identitetsplatform og [OAuth 2.0-godkendelseskodeflow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Denne artikel beskriver, hvordan du programmerer direkte i forhold til flowet til kodetildelning **(PKCE)** i dit program ved hjælp af alle sprog.
- [Microsoft-identitetsplatformen og flowet til OAuth 2.0-klientlegitimationsoplysninger](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Denne artikel beskriver, hvordan du programmerer direkte mod flowet til klientlegitimationsoplysninger i dit program. 
- [Microsoft-identitetsplatform og OAuth 2.0-legitimationsoplysninger](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) for ressourceejer – Denne artikel beskriver, hvordan du programmerer direkte mod **ROPC-flowet** i dit program.
    - Microsoft-identitetsplatformen understøtter kun ROPC for Azure AD-lejere og ikke for personlige konti. Det betyder, at du skal bruge et lejerspecifikt **slutpunkt https://login.microsoftonline.com/{TenantId_or_Name}) (** eller **organisationens** slutpunkt.
    - Personlige konti, der inviteres til en Azure AD-lejer, kan ikke bruge ROPC.
    - Konti, der ikke har adgangskoder, kan ikke logge på via ROPC. I dette scenarie anbefaler vi, at du bruger et andet flow til din app i stedet.
    - Hvis brugerne skal bruge [multifaktorgodkendelse til](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) at logge på programmet, blokeres de.
    - ROPC understøttes ikke i scenarier med [hybrid](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) identitetssammenslutning (f.eks. Azure AD og ADFS, der bruges til at godkende lokale konti). Hvis brugere omdirigeres til en lokal identitetsudbyder, kan Azure AD ikke teste brugernavnet og adgangskoden hos den pågældende identitetsudbyder. [Pass-through-godkendelse](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) understøttes dog med ROPC.
    - En undtagelse til et scenarie med hybrid identitetssammenslutning ville være følgende: Politik for registrering af home Realm med **AllowCloudPasswordValidation** angivet til **SAND** vil gøre det muligt for ROPC-flow at fungere for brugere i organisationsnetværket, når en lokal adgangskode synkroniseres til skyen. Få mere at vide under [Aktivér direkte ROPC-godkendelse af brugere i organisationsnetværket for ældre programmer](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- Microsoft-identitetsplatform og [OAuth 2.0 På](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) vegne af flow – Denne artikel beskriver, hvordan du programmerer direkte mod **OBO-flow (på** vegne af) i dit program.
- Microsoft-identitetsplatformen og [OpenID Connect-protokollen](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Denne artikel viser, hvordan du implementerer OpenID Connect-protokollen uafhængigt af sproget, og den beskriver, hvordan du kan sende og modtage HTTP-meddelelser uden brug af open source-biblioteker fra Microsoft.

**Adgangstokens**

[Adgangstokens for Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Få mere at vide om, hvordan din API kan validere og bruge krav i et adgangstoken. Al dokumentation i denne artikel, undtagen hvor den er angivet, gælder kun for tokens, der er udstedt for API'er, du har registreret. Den gælder ikke for tokens, der er udstedt for Microsoft-ejet API'er, og disse tokens kan heller ikke bruges til at validere, hvordan Microsoft-identitetsplatformen udsteder tokens for en API, du opretter.

**Programkonfiguration**

[Omdiriger restriktioner og begrænsninger for URI (svar URL)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Få mere at vide om, hvordan du konfigurerer din Redirect URI (reply URL). En omdirigerings-URI eller url-adresse er den placering, hvor godkendelsesserveren sender brugeren, når appen er blevet godkendt og tildelt en godkendelseskode eller et adgangstoken. Godkendelsesserveren sender koden eller tokenet til omdirigerings-URI'en. så det er vigtigt, at du registrerer den korrekte placering som en del af appregistreringsprocessen.

**Klargøring af programmer**

[Selvstudium:](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) Udvikling og planlægning af klargøring til et SCIM-slutpunkt – Denne artikel beskriver, hvordan du opbygger et SCIM-slutpunkt og integreres med AAD-klargøringstjenesten.


