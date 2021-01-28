---
title: Problemer med tokenkrav og attributter
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035853"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="92a42-102">Problemer med tokenkrav og attributter</span><span class="sxs-lookup"><span data-stu-id="92a42-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="92a42-103">**Opdater, konfigurer eller fjern token-krav**</span><span class="sxs-lookup"><span data-stu-id="92a42-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="92a42-104">Ved hjælp af Azure Active Directory (Azure AD) kan du tilpasse kravtypen [for](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) rollekravet i det svartoken, du modtager, når du godkender en app.</span><span class="sxs-lookup"><span data-stu-id="92a42-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="92a42-105">Programudviklere kan bruge valgfrie krav i deres Azure AD-programmer til at angive, hvilke krav de ønsker i tokens, der sendes til deres program.</span><span class="sxs-lookup"><span data-stu-id="92a42-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="92a42-106">Du kan finde flere oplysninger [i Angiv valgfrie krav til din app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="92a42-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="92a42-107">[Konfigurere gruppekrav for programmer med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="92a42-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="92a42-108">Hvis du bruger Seamless Single Sign-on i dit program, skal du se tilpassede krav, [der er udstedt i SAML-tokenet til virksomhedsprogrammer.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="92a42-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="92a42-109">**Tilknytning af kravattribut**</span><span class="sxs-lookup"><span data-stu-id="92a42-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="92a42-110">Hvis du vil konfigurere politikken for tilknytning af krav ved hjælp af PowerShell, skal du se Tilpasse krav, der er blevet udsendt i tokens for en bestemt app i [en lejer (forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="92a42-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="92a42-111">Udvidelsesattributter til katalogskemaer gør det muligt at gemme yderligere data i Azure Active Directory på brugerobjekter og andre katalogobjekter, f.eks. grupper, lejeroplysninger, tjeneste principaler.</span><span class="sxs-lookup"><span data-stu-id="92a42-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="92a42-112">Kun udvidelsesattributter på brugerobjekter kan bruges til at udsende krav til programmer.</span><span class="sxs-lookup"><span data-stu-id="92a42-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="92a42-113">[Brug af attributter for katalogskemaudvidelser](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) i krav beskriver, hvordan du bruger attributter for katalogskemaudvidelse til at sende brugerdata til programmer i token-krav.</span><span class="sxs-lookup"><span data-stu-id="92a42-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="92a42-114">Du kan finde flere oplysninger om token-krav i:</span><span class="sxs-lookup"><span data-stu-id="92a42-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="92a42-115">Krav i adgangstokens</span><span class="sxs-lookup"><span data-stu-id="92a42-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="92a42-116">Krav i en id_token</span><span class="sxs-lookup"><span data-stu-id="92a42-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="92a42-117">[Krav, som](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) du kan forvente i id-tokens og adgangstokens udstedt af Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="92a42-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="92a42-118">Saml token-kravreference</span><span class="sxs-lookup"><span data-stu-id="92a42-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
