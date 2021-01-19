---
title: Fejlfinding af gæstebruger problemer
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900950"
---
# <a name="troubleshoot-guest-user-issues"></a>Fejlfinding af gæstebruger problemer

1. Hvis du vil have vejledning i at administrere gæsteadgang til programmer, skal du se [administrere gæsteadgang med Azure ad Access-korrektur](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Tilføje gæstebrugere i din mappe i Azure-portalen](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): i denne hurtigstarter skal du føje en ny gæstebruger til din Azure ad-adresse via Azure-portalen, sende en invitation og se, hvad gæste brugerens indløsnings procedure for indløsning af invitationer ser ud til.
1. [Tilføj en gæstebruger med PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): i denne hurtigstarter skal du bruge kommandoen New-AzureADMSInvitation til at føje én gæstebruger til din Azure-lejer.
1. Du kan få mere at vide om, hvordan du tildeler brugere og grupper til virksomhedsprogrammer i Azure Active Directory (Azure AD), enten fra Azure-portalen eller ved hjælp af PowerShell, under [administrere bruger tildeling for en app i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B-samarbejde fungerer med de fleste apps, der integreres med Azure AD. I denne [artikel](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)gennemgås vejledning til konfiguration af nogle populære SaaS-apps til brug med Azure ad B2B.
1. Som en organisation, der bruger Azure Active Directory (Azure AD) B2B-samarbejdsfunktioner til at invitere gæstebrugere fra partnerorganisationer til Azure AD, kan du nu give disse B2B-brugere adgang til lokale apps. De lokale apps kan bruge SAML-baseret godkendelse eller integreret Windows-godkendelse (IWA) med Kerberos-begrænset delegering (KCD). Hvis du vil have mere at vide, skal du se [TILDELE B2B-brugere i Azure ad Access til dine lokale programmer](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Få mere at vide om, hvordan du [tildeler lokalt administrerede partner konti adgang til Cloud-ressourcer ved hjælp af Azure ad B2B-samarbejde](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).