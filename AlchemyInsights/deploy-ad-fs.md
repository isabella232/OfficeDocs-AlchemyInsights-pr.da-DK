---
title: Installér AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177444"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="94614-102">Installér AD FS</span><span class="sxs-lookup"><span data-stu-id="94614-102">Deploy AD FS</span></span>

<span data-ttu-id="94614-103">En AD FS-installation (Active Directory Federation Services) anvender din lokale infrastruktur til at godkende brugere til Office 365-tjenester.</span><span class="sxs-lookup"><span data-stu-id="94614-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="94614-104">Med logon i organisationsnetværket kan du give brugerne mulighed for at logge på Office 365-tjenester og SAAS-programmer (Software as a Service), der er integreret med Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="94614-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="94614-105">Logon i organisationsnetværket godkender brugere i dit lokale Active Directory via AD FS.</span><span class="sxs-lookup"><span data-stu-id="94614-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="94614-106">Og mens brugerne er på virksomhedens netværk, vil det ikke være nødvendigt at angive deres adgangskoder igen.</span><span class="sxs-lookup"><span data-stu-id="94614-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="94614-107">AD FS-installationsrådgiveren giver dig en trinvis vejledning i installation af en lokal AD FS-infrastruktur, der godkender brugere til Microsoft 365- og Office 365-tjenester. [](https://go.microsoft.com/fwlink/?linkid=2071178)</span><span class="sxs-lookup"><span data-stu-id="94614-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="94614-108">Med denne vejledning kan din organisation gennemse AD FS-komponenter og -krav, købe og installere SSL-certifikater, der er nødvendige for installation, og installere en påkrævet webprogramproxyserver.</span><span class="sxs-lookup"><span data-stu-id="94614-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
