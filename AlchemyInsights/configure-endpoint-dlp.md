---
title: Konfigurer Slutpunkt DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657923"
---
# <a name="configure-endpoint-dlp"></a>Konfigurer Slutpunkt DLP

Microsoft Slutpunkt DLP giver dig mulighed at udvide DLP-beskyttelse og overvågning til følsomme oplysninger på Windows 10-enheder. Når enheder er integreret i enhedsstyring, kan du oprette DLP-politikker for at gennemtvinge beskyttende handlinger for elementer. Aktivitetsoversigten kan bruges til at overvåge aktivitet for følsomme elementer. Du kan få mere at vide under [Tilføjelse af enheder til enhedsstyring](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Sådan kommer du i gang med Slutpunkt DLP:

- Sørg for, at du har den rette SKU/abonnementslicens. Du kan finde flere oplysninger i[Licenser til SKU/abonnementer](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontrollér de tilladelser, der kræves for at aktivere enhedsstyring, få adgang til onboarding-siden eller aktivere/deaktivere overvågning af enheder. Du kan finde flere oplysninger under [Tilladelser](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Føj enheder til Enhedsstyring ved at følge proceduren for onboarding af enheder. Du kan få mere at vide i [Tilføjelse af enheder](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Opret DLP-politikker for at beskytte dine følsomme elementer. Du kan få mere at vide i [Scenarier med Slutpunkt DLP-politik](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Du kan finde flere oplysninger om Microsoft Endpoint DLP i [Få mere at vide om forebyggelse af datatab for Microsoft 365 Endpoint (prøveversion)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Vigtige trin til indsamling af data, hvis der er behov for støtte:**

1. Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Kør værktøjet som administrator fra cmd-vinduet:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Når du bliver bedt om det, angiv det antal minutter, der skal bruges til at indsamle **sporinger:**, angiv det antal minutter, der kræves for at køre scenariet.
1. Kør scenariet.

Indsaml zip-filoutput for at give det til supportmedarbejderen.
