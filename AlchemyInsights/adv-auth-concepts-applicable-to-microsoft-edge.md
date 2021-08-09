---
title: Avancerede godkendelseskoncepter, der gælder for Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934359"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avancerede godkendelseskoncepter, der gælder for Microsoft Edge

Følgende er de avancerede godkendelseskoncepter, der gælder for Microsoft Edge:

**Proactive Authentication**

Når du aktiverer [politikken ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) vil Microsoft Edge proaktivt godkende brugere, der er logget på, via Microsoft-tjenester. Den vil med jævne mellemrum bruge en onlinetjeneste til at kontrollere, om der er et opdateret manifest, der indeholder den konfiguration, der styrer Proaktiv godkendelse.

Fordele: Proactive Authentication enables authentication to key services, such as Office New Tab Page. Hvis Bing bruges som søgemaskine, forbedrer Proactive Authentication også ydeevnen af adresselinjen og hjælper med at generere søgeresultater, der er tilpasset behovene i din virksomhed.

**Windows Hello CredUI til NTLM-godkendelse**

Hvis enkelt logon (SSO) ikke er tilgængelig, når et websted forsøger at logge på brugeren via mekanismen NTLM eller forhandl, gør denne funktion det muligt for brugeren at dele os-legitimationsoplysningerne med webstedet og opfylde godkendelsesudfordringen ved hjælp af Windows Hello Cred UI. Dette logonflow vises kun i Windows 10 og kun for brugere, der ikke får SSO under en NTLM- eller en forhandl-udfordring.

**Brug gemte adgangskoder til at logge på automatisk**

Brugere, der gemmer adgangskoder Microsoft Edge, kan aktivere automatisk logon på websteder, hvor de har gemt legitimationsoplysninger. Brugere kan slå denne funktion til eller fra i edge://settings/passwords, og du kan konfigurere den i [politikkerne for password manager.](https://go.microsoft.com/fwlink/?linkid=2134622)
