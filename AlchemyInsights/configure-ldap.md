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
# <a name="configure-ldap"></a>Konfigurere LDAP

Hvis du vil konfigurere LDAP, skal du gøre følgende:

1. Kontrollér domænets tilstand på Azure- [portalen](https://aka.ms/aadds-health).
1. Sørg for, at der findes et gyldigt Azure AD-abonnement, og Azure AD-domæne tjenester er blevet aktiveret.
1. Det certifikat, der er påkrævet for at aktivere sikker LDAP, skal fås fra et offentligt nøglecenter, der er tillid til, eller være et selvsigneret certifikat.
1. Sørg for, at certifikatet følger de nødvendige [retningslinjer](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Ugyldigt certifikat**
1. Hvis du vil forny et certifikat, skal du følge trinnene for at oprette et nyt certifikat og overføre: [Konfigurer LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Hvis du vil løse et kendt problem med sikre LDAP-beskeder i Azure Active Directory-domæne tjenester, skal du se [løs LDAP-beskeder](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
