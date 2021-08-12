---
title: Fejlfinding af problemer med gæstebrugere
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939373"
---
# <a name="troubleshoot-guest-user-issues"></a>Fejlfinding af problemer med gæstebrugere

1. Du kan finde en vejledning til administration af gæsteadgang til programmer [i Administrer gæsteadgang med Azure AD-adgangsvurderinger.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Føj gæstebrugere](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)til dit katalog i Azure-portalen: I denne hurtig start skal du føje en ny gæstebruger til dit Azure AD-katalog via Azure-portalen, sende en invitation og se, hvordan gæstebrugerens indløsningsproces ser ud.
1. [Tilføj en gæstebruger med PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)I denne hurtig start skal du bruge kommandoen New-AzureADMSInvitation til at føje én gæstebruger til din Azure-lejer.
1. Hvis du vil lære, hvordan du tildeler brugere og grupper til virksomhedsprogrammer i Azure Active Directory (Azure AD), enten fra Azure-portalen eller ved hjælp af PowerShell, skal du se Administrer brugertildeling for en [app i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) fungerer B2B-samarbejde med de fleste apps, der integreres med Azure AD. I denne [artikel gennemgår](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)vi instruktioner til konfiguration af nogle populære SaaS-apps til brug med Azure AD B2B.
1. Som en organisation, der bruger Azure Active Directory (Azure AD) B2B-samarbejdsfunktioner til at invitere gæstebrugere fra partnerorganisationer til din Azure AD, kan du nu give disse B2B-brugere adgang til lokale apps. Disse lokale apps kan bruge SAML-baseret godkendelse eller IWA (Integrated Windows Authentication) med Kerberos' begrænsningsdelegering (KCD). Få mere at vide under [Giv B2B-brugere i Azure AD adgang til dine programmer i det lokale miljø.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Få mere at vide [om, hvordan du giver lokalt administrerede partnerkonti adgang til skyressourcer ved hjælp af Azure AD B2B-samarbejde.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)