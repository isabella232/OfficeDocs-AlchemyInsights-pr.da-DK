---
title: Avancerede godkendelses koncepter, der gælder for Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573330"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avancerede godkendelses koncepter, der gælder for Microsoft Edge

Følgende er de avancerede godkendelses koncepter, der gælder for Microsoft Edge:

**Proaktiv godkendelse**

Når du aktiverer [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -politikken, forsøger Microsoft Edge proaktivt at godkende brugere, der er logget på, via Microsoft-tjenester. Med jævne mellemrum bruges en onlinetjeneste til at kontrollere, om der er et opdateret manifest, der indeholder konfigurationen til proaktiv godkendelse.

Fordele: proaktiv godkendelse giver mulighed for godkendelse af nøgle tjenester, f. eks den nye faneside i Office. Hvis Bing også bruges som søgemaskine, forbedrer proaktiv godkendelse ydeevnen for adresselinjen og hjælper med at oprette søgeresultater, der er tilpasset din virksomheds behov.

**Windows Hello CredUI til NTLM-godkendelse**

Hvis enkeltlogon (SSO) ikke er tilgængelig, når et websted forsøger at logge på brugeren via NTLM-eller Negotiate-mekanismen, giver brugeren mulighed for at dele OS-legitimationsoplysninger med webstedet og for at opfylde godkendelses udfordringen ved hjælp af BRUGERGRÆNSEFLADEN i Windows Hello-legitimationsoplysninger. Dette tilmeldings forløb vises kun i Windows 10 og kun for brugere, der ikke får SSO under en NTLM-eller en Negotiate-udfordring.

**Brug gemte adgangskoder til at logge på automatisk**

Brugere, der gemmer adgangskoder i Microsoft Edge, kan aktivere automatisk logon på websteder, hvor de har gemt dine legitimationsoplysninger. Brugere kan slå denne funktion til eller fra i edge://settings/passwords, og du kan konfigurere den i politikker for [adgangskodestyring](https://go.microsoft.com/fwlink/?linkid=2134622) .
