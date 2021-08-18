---
title: Konfigurer LDAP
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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090406"
---
# <a name="configure-ldap"></a>Konfigurer LDAP

Gør følgende for at konfigurere LDAP:

1. Kontrollér domænets tilstand på [Azure-portalen.](https://aka.ms/aadds-health)
1. Sørg for, at et gyldigt Azure AD-abonnement er tilgængeligt, og at Azure AD-domænetjenester er aktiveret.
1. Det certifikat, der kræves for at aktivere sikker LDAP, skal hentes fra et offentligt nøglecenter, der er tillid til, eller være et selv signeret certifikat.
1. Sørg for, at certifikatet følger de nødvendige [retningslinjer](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Ugyldigt certifikat**
1. Hvis du vil forny et certifikat, skal du følge trinnene for at oprette et nyt certifikat og genindlæse: [Konfigurer LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Se Løs LDAP-beskeder for at løse et kendt problem med Secure [LDAP-beskeder](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)i Azure Active Directory Domain Services.
