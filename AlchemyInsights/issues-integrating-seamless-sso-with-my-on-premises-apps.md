---
title: Problemer med integrering af Seamless SSO med mine lokale apps
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028286"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemer med integrering af Seamless SSO med mine lokale apps

Hvis du vil foretage fejlfinding af problemer med integrering af Seamless SSO i programmer i det lokale miljø, skal du gøre følgende:

**Anbefalede trin**

1. Hvis du vil **konfigurere et** lokalt program til enkelt logon via programproxy, skal du se Adgangskodevældning for enkelt logon med  [programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Fejlfinding af problemer** med programproxy: Vi [anbefaler,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)at du starter med at gennemgå fejlfindingsflowet, Fejlfinding af problemer med programproxyforbindelse for at afgøre, om programproxyforbindelser er konfigureret korrekt. Hvis du stadig har problemer med at oprette forbindelse til programmet, skal du følge fejlfindingstrinnene i [Fejlfinding af problemer med programproxyprogrammet.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Du kan [identificere CORS-problemer ved](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) hjælp af følgende browser-fejlfindingsværktøjer:
    1. Start browseren, og gå til webappen.
    1. Tryk **på F12** for at få adgang til fejlfindingskonsollen.
    1. Prøv at genskabe transaktionen, og gennemse konsolmeddelelsen. En CORS-overtrædelse giver en konsolfejl om oprindelse.
    1. Nogle CORS-problemer kan ikke løses, f.eks. når din app omdirigerer til en login.microsoftonline.com godkendelse, og adgangstoken udløber. Så mislykkes CORS-opkaldet. En løsning i dette scenarie er at forlænge en adgangstokens levetid for at forhindre, at den udløber under en brugers session. Du kan finde flere oplysninger om, hvordan du gør dette, [under Konfigurerbar tokenlevetid i Microsoft-identitetsplatform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Anbefalede dokumenter**

- [Sådan konfigureres enkelt logon til et programproxyprogram](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML-enkelt logon til lokale programmer med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Forstå og løse problemer Azure Active Directory programproxyen CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Fejlfinding af konfigurationer af begrænset delegering af Kerberos for programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)