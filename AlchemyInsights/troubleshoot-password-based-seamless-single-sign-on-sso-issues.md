---
title: Fejlfinding af adgangskodebaserede problemer med enkelt logon (Seamless Single Sign-on)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972818"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Fejlfinding af adgangskodebaserede problemer med enkelt logon (Seamless Single Sign-on)

Hvis du vil lære det grundlæggende for adgangskodebaseret SSO, skal du [se Adgangskodebaseret godkendelse med Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfigurere adgangskodebaseret SSO**

1. [Konfigurer adgangskodebaseret enkelt logon – Denne](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) artikel indeholder flere oplysninger om den adgangskodebaserede SSO-indstilling. Hvis det program, du tilføjer, kræver brugerdefineret konfiguration, og du skal bruge adgangskodebaseret SSO, er denne artikel for dig.
2. [Konfigurer adgangskodebaseret enkelttegn for programmer i det pågældende program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Programproxy understøtter flere tilstandene for enkelt sign-on. Adgangskodebaseret logon er beregnet til programmer, der bruger en kombination af brugernavn/adgangskode til godkendelse. Når du konfigurerer adgangskodebaseret logon for dit program, skal brugerne logge på det lokale program én gang. Derefter gemmer Azure Active Directory logonoplysningerne og leverer dem automatisk til programmet, når dine brugere får fjernadgang til dem.
    - Du bør allerede have publiceret og testet din app med programproxy. Hvis ikke, skal du følge trinnene i Publicere programmer ved hjælp af [Azure AD Application Proxy,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) og derefter fortsætte din konfiguration af adgangskodebaseret SSO til programmer i det offentlige.

Hvis du vil foretage fejlfinding af adgangskodebaseret SSO, skal du [se Fejlfinding af adgangskodebaseret enkelt logon i Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
