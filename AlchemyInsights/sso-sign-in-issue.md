---
title: Problemfri logonproblemer for SSO-brugere
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935094"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problemfri logonproblemer for SSO-brugere

Når brugeren er godkendt, cachelagrer browseren brugerens legitimationsoplysninger, så programmet automatisk logger på med den samme konto i den samme browser. Dette kan gøre det svært for en anden bruger eller en enkelt bruger at logge på flere konti på én enhed. Sådan løser du dette: 1. Prøv at logge på en anden browser. 2. Ryd browserens cache og/eller cookies, og prøv at logge på igen.

Hvis du stadig oplever problemer med logon, anbefaler vi følgende for at diagnosticere og automatisere trinnene til løsning:

1. Installer Secure [Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) til Mine apps for at hjælpe Azure Active Directory (Azure AD) med at levere bedre diagnose og løsninger, når du bruger testoplevelsen i Azure-portalen.
2. Genskab fejlen ved hjælp af testoplevelsen på siden til appkonfiguration i Azure-portalen. Hvis du vil have mere at vide, [skal du se Fejlfinding af SAML-baserede programmer til enkeltloga.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Hvis du bruger testoplevelsen i Azure-portalen med min apps sikre browserudvidelse, kan du **springe trin 4 over.**
4. Sådan åbner du den SAML-baserede konfigurationsside for enkelt logon:
    - Åbn [Azure-portalen,](https://portal.azure.com/) og log på som **global administrator** eller **Coadmin.**
    - Åbn **Azure Active Directory-udvidelsen** ved at **vælge Alle** tjenester øverst i den primære venstre navigationsmenu.
    - Skriv "Azure Active Directory" i filtersøgefeltet, og vælg **Azure Active Directory-elementet.**
    - Vælg **Enterprise Applications** i azure Active Directory-navigationsmenuen til venstre.
    - Vælg **Alle programmer for** at få vist en liste over alle dine programmer. Hvis det ønskede program ikke vises her,  kan du bruge filterkontrolelementet øverst  på listen Alle programmer og angive indstillingen Vis til **Alle programmer.** 
    - Vælg det program, du vil konfigurere til enkelt logon.
    - Når programmet er indlæst, **skal du vælge Enkelt** logon i programmets venstre navigationsmenu.
    - Vælg **SAML-baseret SSO.**
5. Baseret på fejlen kan du få mere at vide om de anbefalede trin, du skal følge, ved at se Problemer med at logge på [SAML-baserede](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)apps, der er konfigureret til enkelt logon.
6. Hvis du vil foretage fejlfinding af andre problemer med brugertegn, skal du se følgende vejledning:
    - [Single Sign-On SAML-protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Sådan foretager du fejlfinding af logonfejl ved hjælp af Azure Active Directory-rapporter](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Uventet samtykkeprompt](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Fejl i brugersamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemer med at logge på fra Mine apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Fejl på programmets logonside](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problem med at logge på en Microsoft-app](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
