---
title: Problemer med SSO-forbindelse
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084340"
---
# <a name="sso-connection-issues"></a>Problemer med SSO-forbindelse

1. Følg [Quickstart: Konfigurer egenskaberne for en programvejledning](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) for at konfigurere dit program.
2. Afhængigt af det program [og indstillingen Enkelt logon, du](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) har valgt, skal du følge den relevante vejledning nedenfor:
    - Hvis du vil **konfigurere** et lokalt program til **SAML-baseret enkelttegn på**, skal du se [SAML single-sign-on for](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)lokale programmer med programproxy.
    - Hvis du vil **konfigurere et skybaseret** **program til adgangskodebaseret enkelttegn på**, skal du se Konfigurere  [enkeltadgangskode til](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Hvis du vil **konfigurere et** lokalt program til enkelt logon via programproxy, skal du se Adgangskodevældning for enkelt logon med  [programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Fejlfinding af problemer med** programproxy: Vi [anbefaler,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)at du starter med at gennemgå fejlfindingsflowet, Fejlfinding af problemer med programproxyforbindelse for at finde ud af, om programproxyforbindelser er konfigureret korrekt. Hvis du stadig har problemer med at oprette forbindelse til programmet, skal du følge fejlfindingsflowet i [Fejlfinding af programproxyprogrammets problemer.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Du kan [identificere CORS-problemer ved](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) hjælp af browser-fejlfindingsværktøjer:
    - Start browseren, og gå til webappen.
    - Tryk **på F12** for at få adgang til fejlfindingskonsollen.
    - Prøv at genskabe transaktionen, og gennemse konsolmeddelelsen. En CORS-overtrædelse giver en konsolfejl om oprindelse.
    - Nogle CORS-problemer kan ikke løses, f.eks. når din app omdirigerer til login.microsoft.com godkendelse, og adgangstoken udløber. Så mislykkes CORS-opkaldet. En løsning i dette scenarie er at forlænge en adgangstokens levetid for at forhindre, at den udløber under en brugers session. Du kan finde flere oplysninger om, hvordan du gør dette, [under Konfigurerbar tokenlevetid i Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Fejlfinding af SAML-baseret** enkelt logon: Vi anbefaler, at du kontrollerer Problemer med at logge på [SAML-baserede](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)apps, der er konfigureret til enkelt logon, for at finde løsninger på de problemer, der mest sandsynligt vil opstå.
5. **Fejlfinding af adgangskodebaseret** enkelt logon: Vi anbefaler, at du kontrollerer Fejlfinding af adgangskodebaseret enkelt logon til [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)for at finde løsninger på de problemer, der mest sandsynligt vil opstå.
6. Hvis du har forbindelsesproblemer, når du bruger et VPN, skal du se Sådan bruger du [enkelttegn på (SSO) over VPN Wi-Fi-forbindelser.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
