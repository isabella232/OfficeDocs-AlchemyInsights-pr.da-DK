---
title: Problemer med at integrere problemfrit SSO med mine lokale apps
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868652"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemer med at integrere problemfrit SSO med mine lokale apps

Hvis du vil foretage fejlfinding af problemer med at integrere problemfrit SSO med programmer i det lokale miljø, skal du gøre følgende:

**Anbefalede trin**

1. Hvis du vil konfigurere et **lokalt program** til **enkeltlogon via proxyen**, skal du se bruge [adgangskode til at logge på med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Fejlfinding af problemer med programproxy**: Vi anbefaler, at du starter med at gennemgå fejlfindingsprocessen, [fejlfinding af problemer med programproxy forbindelse](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), for at finde ud af, om proxyforbindelser er konfigureret korrekt. Hvis du stadig har problemer med at oprette forbindelse til programmet, skal du følge fejlfindingstrinnene i problemer med program [proxy programmet til fejlfinding](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Du kan [identificere Cors-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ved hjælp af følgende fejlfindingsværktøjer i browseren:
    1. Start browseren, og gå til web-appen.
    1. Tryk på **F12** for at få vist fejlfindings konsollen.
    1. Prøv at reproducere transaktionen, og gennemse konsol meddelelsen. En CORS-fejl giver en konsol fejl om oprindelse.
    1. Nogle CORS-problemer kan ikke løses, f. eks når din app omdirigerer til login.microsoftonline.com for at godkende, og Access-tokenet udløber. CORS-opringningen mislykkes derefter. En løsning på dette scenario er at forlænge levetiden for det pågældende adgangstoken for at forhindre, at det udløber under en brugers session. Du kan finde flere oplysninger om, hvordan du gør dette, under [konfigurerbare levetid for tokens i Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Anbefalede dokumenter**

- [Sådan konfigureres Single Sign-on til et program proxy program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML enkeltlogon for lokale programmer med program proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Forstå og løse problemer i forbindelse med Azure Active Directory-program proxy CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Foretag fejlfinding af konfigurationer af begrænsede Kerberos-dele for program proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)