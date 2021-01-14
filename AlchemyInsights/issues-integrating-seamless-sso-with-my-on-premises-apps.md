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
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="fdc79-102">Problemer med at integrere problemfrit SSO med mine lokale apps</span><span class="sxs-lookup"><span data-stu-id="fdc79-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="fdc79-103">Hvis du vil foretage fejlfinding af problemer med at integrere problemfrit SSO med programmer i det lokale miljø, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="fdc79-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="fdc79-104">**Anbefalede trin**</span><span class="sxs-lookup"><span data-stu-id="fdc79-104">**Recommended steps**</span></span>

1. <span data-ttu-id="fdc79-105">Hvis du vil konfigurere et **lokalt program** til **enkeltlogon via proxyen**, skal du se bruge [adgangskode til at logge på med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="fdc79-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="fdc79-106">**Fejlfinding af problemer med programproxy**: Vi anbefaler, at du starter med at gennemgå fejlfindingsprocessen, [fejlfinding af problemer med programproxy forbindelse](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), for at finde ud af, om proxyforbindelser er konfigureret korrekt.</span><span class="sxs-lookup"><span data-stu-id="fdc79-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="fdc79-107">Hvis du stadig har problemer med at oprette forbindelse til programmet, skal du følge fejlfindingstrinnene i problemer med program [proxy programmet til fejlfinding](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="fdc79-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="fdc79-108">Du kan [identificere Cors-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ved hjælp af følgende fejlfindingsværktøjer i browseren:</span><span class="sxs-lookup"><span data-stu-id="fdc79-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="fdc79-109">Start browseren, og gå til web-appen.</span><span class="sxs-lookup"><span data-stu-id="fdc79-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="fdc79-110">Tryk på **F12** for at få vist fejlfindings konsollen.</span><span class="sxs-lookup"><span data-stu-id="fdc79-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="fdc79-111">Prøv at reproducere transaktionen, og gennemse konsol meddelelsen.</span><span class="sxs-lookup"><span data-stu-id="fdc79-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="fdc79-112">En CORS-fejl giver en konsol fejl om oprindelse.</span><span class="sxs-lookup"><span data-stu-id="fdc79-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="fdc79-113">Nogle CORS-problemer kan ikke løses, f. eks når din app omdirigerer til login.microsoftonline.com for at godkende, og Access-tokenet udløber.</span><span class="sxs-lookup"><span data-stu-id="fdc79-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="fdc79-114">CORS-opringningen mislykkes derefter.</span><span class="sxs-lookup"><span data-stu-id="fdc79-114">The CORS call then fails.</span></span> <span data-ttu-id="fdc79-115">En løsning på dette scenario er at forlænge levetiden for det pågældende adgangstoken for at forhindre, at det udløber under en brugers session.</span><span class="sxs-lookup"><span data-stu-id="fdc79-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="fdc79-116">Du kan finde flere oplysninger om, hvordan du gør dette, under [konfigurerbare levetid for tokens i Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="fdc79-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="fdc79-117">**Anbefalede dokumenter**</span><span class="sxs-lookup"><span data-stu-id="fdc79-117">**Recommended documents**</span></span>

- [<span data-ttu-id="fdc79-118">Sådan konfigureres Single Sign-on til et program proxy program</span><span class="sxs-lookup"><span data-stu-id="fdc79-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="fdc79-119">SAML enkeltlogon for lokale programmer med program proxy</span><span class="sxs-lookup"><span data-stu-id="fdc79-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="fdc79-120">Forstå og løse problemer i forbindelse med Azure Active Directory-program proxy CORS</span><span class="sxs-lookup"><span data-stu-id="fdc79-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="fdc79-121">Foretag fejlfinding af konfigurationer af begrænsede Kerberos-dele for program proxy</span><span class="sxs-lookup"><span data-stu-id="fdc79-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)