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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935088"
---
# <a name="sso-connection-issues"></a>Problemer med SSO-forbindelse

1. Følg [startvejledningen: Konfigurer egenskaberne for en programvejledning](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) for at konfigurere dit program.
2. Afhængigt af programmet [og indstillingen Enkelt logon, du har](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) valgt, skal du følge den relevante vejledning nedenfor:
    - Hvis du vil **konfigurere** et lokalt program til **SAML-baseret** enkelt-logon, skal du se [SAML single-sign-on for](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)lokale programmer med programproxy.
    - Hvis du vil **konfigurere et skybaseret** **program til adgangskodebaseret enkelt logon,** skal du se [Konfigurer enkeltadgangskode.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Hvis du vil **konfigurere et** lokalt program **til** enkelt logon via programproxy, skal du se Adgangskodekryptering for enkelt logon [med programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Fejlfinding af problemer** med programproxy: Vi anbefaler, at du starter med at gennemgå fejlfindingsflowet, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)foretager fejlfinding af problemer med programproxyforbindelse for at afgøre, om programproxyforbindelser er konfigureret korrekt. Hvis du stadig har problemer med at oprette forbindelse til programmet, skal du følge fejlfindingsflowet i [programproxyprogrammet](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)Fejlfinding. Du kan [identificere CORS-problemer ved](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) hjælp af værktøjerne til fejlfinding i browseren:
    - Start browseren, og gå til webappen.
    - Tryk **på F12** for at få adgang til fejlfindingskonsollen.
    - Prøv at genskabe transaktionen, og gennemse konsolmeddelelsen. En CORS-overtrædelse giver en konsolfejl om oprindelse.
    - Nogle CORS-problemer kan ikke løses, f.eks. når din app omdirigerer til login.microsoft.com godkendelse, og adgangstokenet udløber. Cors-opkaldet mislykkes derefter. En midlertidig løsning på dette scenarie er at forlænge levetiden for adgangstokenet for at forhindre, at det udløber under en brugers session. Du kan finde flere oplysninger om, hvordan du gør dette, under [Konfigurerbar tokenlevetid i Microsoft-identitetsplatformen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **Fejlfinding af SAML-baseret enkelt** logon: Vi anbefaler, at du kontrollerer problemer med at logge på [SAML-baserede](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)apps, der er konfigureret til enkelt logon, for at finde løsninger på de problemer, der mest sandsynligt vil opstå.
5. **Fejlfinding af adgangskodebaseret** enkelt-logon: Vi anbefaler, at du kontrollerer fejlfinding af adgangskodebaseret enkelt logon i [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)for at finde løsninger på de problemer, der mest sandsynligt vil opstå.
6. Hvis du har forbindelsesproblemer, når du bruger et VPN, skal du se, hvordan du bruger [enkelt-logon (SSO) over VPN Wi-Fi-forbindelser.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
