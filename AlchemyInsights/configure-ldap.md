---
title: Konfigurere LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884957"
---
# <a name="configure-ldap"></a><span data-ttu-id="89af5-102">Konfigurere LDAP</span><span class="sxs-lookup"><span data-stu-id="89af5-102">Configure LDAP</span></span>

<span data-ttu-id="89af5-103">Hvis du vil konfigurere LDAP, skal du gøre følgende:</span><span class="sxs-lookup"><span data-stu-id="89af5-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="89af5-104">Kontrollér domænets tilstand på Azure- [portalen](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="89af5-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="89af5-105">Sørg for, at der findes et gyldigt Azure AD-abonnement, og Azure AD-domæne tjenester er blevet aktiveret.</span><span class="sxs-lookup"><span data-stu-id="89af5-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="89af5-106">Det certifikat, der er påkrævet for at aktivere sikker LDAP, skal fås fra et offentligt nøglecenter, der er tillid til, eller være et selvsigneret certifikat.</span><span class="sxs-lookup"><span data-stu-id="89af5-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="89af5-107">Sørg for, at certifikatet følger de nødvendige [retningslinjer](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="89af5-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="89af5-108">**Ugyldigt certifikat**</span><span class="sxs-lookup"><span data-stu-id="89af5-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="89af5-109">Hvis du vil forny et certifikat, skal du følge trinnene for at oprette et nyt certifikat og overføre: [Konfigurer LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="89af5-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="89af5-110">Hvis du vil løse et kendt problem med sikre LDAP-beskeder i Azure Active Directory-domæne tjenester, skal du se [løs LDAP-beskeder](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="89af5-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
