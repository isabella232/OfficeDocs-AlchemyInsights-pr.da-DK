---
title: Konfiguration af appproxy
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
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951559"
---
# <a name="app-proxy-configuration"></a>Konfiguration af appproxy

1. For at forstå, hvordan du konfigurerer et programproxyprogram i Azure AD for at vise dine programmer i det lokale miljø til skyen, skal du se Sådan konfigureres [et programproxyprogram](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Enkelt logon giver dine brugere mulighed for at få adgang til et program uden at godkende flere gange. Det gør det muligt at udføre enkeltgodkendelse i skyen mod Azure Active Directory og gør det muligt for tjenesten eller Connector at udgive sig for at være brugeren og udføre eventuelle yderligere godkendelsesudfordringer fra programmet. Du kan få mere at vide [under Sådan konfigureres enkelt logon til et programproxyprogram.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Brug [denne artikel til at](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) foretage fejlfinding af almindelige problemer, som folk står over for, når de opretter et nyt programproxyprogram.
4. Hvis du har et problem med at konfigurere back-end-godkendelse i dit program, kan det være nødvendigt at foretage fejlfinding af [Kerberos begrænsede delegeringskonfigurationer for](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) programproxy eller følge en vejledning til konfiguration af programmet med [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) for at løse problemet.
