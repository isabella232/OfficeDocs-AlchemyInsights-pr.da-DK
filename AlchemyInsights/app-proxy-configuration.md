---
title: Konfiguration af app-proxy
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884945"
---
# <a name="app-proxy-configuration"></a>Konfiguration af app-proxy

1. Hvis du vil vide, hvordan du konfigurerer et programproxy program i Azure AD for at vise dine lokale programmer i skyen, skal du se [Sådan konfigurerer du et programproxy program](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Enkeltlogon (SSO) gør det muligt for dine brugere at få adgang til et program uden at godkende flere gange. Det giver mulighed for, at der opstår en enkelt godkendelse i skyen, oversættes til Azure Active Directory, og tjenesten eller forbindelseskomponenten til at repræsentere brugeren for at fuldføre eventuelle yderligere godkendelses udfordringer fra programmet. Hvis du vil have mere at vide, skal du se [Sådan konfigurerer du Single Sign-on til et program proxy program](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Brug [denne artikel](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) til at foretage fejlfinding af almindelige problemer, der opstår, når man opretter et nyt programproxy program.
4. Hvis du har problemer med at konfigurere back-end-godkendelse til dit program, kan det være nødvendigt at [foretage fejlfinding af Kerberos-begrænsede delegering af program proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) eller følge vejledningen i [konfiguration af program med PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) for at løse problemet.
