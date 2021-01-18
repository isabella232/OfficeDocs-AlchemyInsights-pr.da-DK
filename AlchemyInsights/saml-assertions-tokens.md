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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="9bae6-102">SAML antagelser (tokens)</span><span class="sxs-lookup"><span data-stu-id="9bae6-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="9bae6-103">SAML-tokens (Security Assertion Markup Language) er XML repræsentationer af krav.</span><span class="sxs-lookup"><span data-stu-id="9bae6-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="9bae6-104">Som standard bruger du SAML tokens Windows Communication Foundation (WCF) i forbundne sikkerheds scenarier, udstedes tokens.</span><span class="sxs-lookup"><span data-stu-id="9bae6-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="9bae6-105">Du kan få mere at vide under [Saml tokens og krav](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="9bae6-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="9bae6-106">Microsoft Identity platform udsender flere typer af sikkerhedstokens under behandlingen af hvert godkendelsesforløb.</span><span class="sxs-lookup"><span data-stu-id="9bae6-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="9bae6-107">[Saml tokens Claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beskriver formatet, sikkerhedsegenskaberne og indholdet af Saml 2,0-tokens.</span><span class="sxs-lookup"><span data-stu-id="9bae6-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="9bae6-108">Følg vejledningen i [konfigurerbare tokens levetid i Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) for at forstå, hvordan du konfigurerer levetid for tokens.</span><span class="sxs-lookup"><span data-stu-id="9bae6-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="9bae6-109">Følg de trin, der er beskrevet i [denne artikel](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) , for at forstå, hvordan du KONFIGURERER Azure ad Saml token-kryptering.</span><span class="sxs-lookup"><span data-stu-id="9bae6-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="9bae6-110">I Azure AD kan du konfigurere indstillinger for certifikat signering og signerings algoritmen for certifikater.</span><span class="sxs-lookup"><span data-stu-id="9bae6-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="9bae6-111">Hvis du vil have mere at vide, skal du se [Avancerede indstillinger for certifikat signering i APPEN Saml token for Gallery i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="9bae6-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
