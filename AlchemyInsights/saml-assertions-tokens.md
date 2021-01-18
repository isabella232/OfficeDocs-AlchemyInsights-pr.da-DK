---
title: SAML antagelser (tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884981"
---
# <a name="saml-assertions-tokens"></a>SAML antagelser (tokens)

1. SAML-tokens (Security Assertion Markup Language) er XML repræsentationer af krav. Som standard bruger du SAML tokens Windows Communication Foundation (WCF) i forbundne sikkerheds scenarier, udstedes tokens. Du kan få mere at vide under [Saml tokens og krav](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Microsoft Identity platform udsender flere typer af sikkerhedstokens under behandlingen af hvert godkendelsesforløb. [Saml tokens Claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beskriver formatet, sikkerhedsegenskaberne og indholdet af Saml 2,0-tokens.
3. Følg vejledningen i [konfigurerbare tokens levetid i Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) for at forstå, hvordan du konfigurerer levetid for tokens.
4. Følg de trin, der er beskrevet i [denne artikel](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) , for at forstå, hvordan du KONFIGURERER Azure ad Saml token-kryptering.
5. I Azure AD kan du konfigurere indstillinger for certifikat signering og signerings algoritmen for certifikater. Hvis du vil have mere at vide, skal du se [Avancerede indstillinger for certifikat signering i APPEN Saml token for Gallery i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
