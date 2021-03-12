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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714709"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Fejlfinding af adgangskodebaserede problemer med enkelt logon (Seamless Single Sign-on)

Du kan få mere at vide om det grundlæggende ved adgangskodebaseret SSO [under Adgangskodebaseret godkendelse med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurere adgangskodebaseret SSO**

1. [Konfigurer adgangskodebaseret enkelt-logon – Denne](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) artikel indeholder flere oplysninger om den adgangskodebaserede SSO-indstilling. Hvis det program, du tilføjer, kræver brugerdefineret konfiguration, og du skal bruge adgangskodebaseret SSO, er denne artikel for dig.
2. [Konfigurer adgangskodebaseret enkelttegn til apps i det pågældende program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Programproxy understøtter flere tilstande til enkelt logon. Adgangskodebaseret logon er beregnet til programmer, der bruger en kombination af brugernavn/adgangskode til godkendelse. Når du konfigurerer adgangskodebaseret logon til dit program, skal brugerne logge på det lokale program én gang. Derefter gemmer Azure Active Directory logonoplysningerne og leverer dem automatisk til programmet, når dine brugere får adgang til dem eksternt.
    - Du bør allerede have publiceret og testet din app med programproxy. Hvis ikke, skal du følge trinnene i Publicer programmer ved hjælp af Azure AD-programproxy og derefter fortsætte din konfiguration af adgangskodebaseret SSO til apps i det pågældende program. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)

Hvis du vil foretage fejlfinding af adgangskodebaseret SSO, skal du [se Fejlfinding af adgangskodebaseret enkelt logon i Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
