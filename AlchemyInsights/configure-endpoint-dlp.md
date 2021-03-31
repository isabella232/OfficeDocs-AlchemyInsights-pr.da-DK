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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402410"
---
# <a name="configure-endpoint-dlp"></a>Konfigurer Slutpunkt DLP

Microsoft Slutpunkt DLP giver dig mulighed at udvide DLP-beskyttelse og overvågning til følsomme oplysninger på Windows 10-enheder. Når enheder er integreret i enhedsstyring, kan du oprette DLP-politikker for at gennemtvinge beskyttende handlinger for elementer. Aktivitetsoversigten kan bruges til at overvåge aktivitet for følsomme elementer. Du kan få mere at vide under [Tilføjelse af enheder til enhedsstyring](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Sådan kommer du i gang med Slutpunkt DLP:

- Sørg for, at du har den rette SKU/abonnementslicens. Du kan finde flere oplysninger i[Licenser til SKU/abonnementer](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontrollér de tilladelser, der kræves for at aktivere enhedsstyring, få adgang til onboarding-siden eller aktivere/deaktivere overvågning af enheder. Du kan finde flere oplysninger under [Tilladelser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Føj enheder til Enhedsstyring ved at følge proceduren for onboarding af enheder. Hvis du mangler indstillingen Tilføjelse af enhed (forhåndvisning) under M365 Compliance  **Settings**, skal du bekræfte, at du har den korrekte licens og de tilladelser, der henvises til ovenfor. Du kan få mere at vide i [Tilføjelse af enheder](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Opret DLP-politikker for at beskytte dine følsomme elementer. Du kan få mere at vide i [Scenarier med Slutpunkt DLP-politik](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Du kan finde flere oplysninger om Microsoft Endpoint DLP i [Få mere at vide om forebyggelse af datatab for Microsoft 365 Endpoint (prøveversion)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Vigtige trin til indsamling af data, hvis der er behov for støtte:**

1. Hent prøveversionen af MDATP-klientanalyse fra [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Kør værktøjet som administrator fra cmd-vinduet:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Når du bliver bedt om at "angive antal minutter til indsamling af spor: ", skal du angive det antal minutter, der kræves for at køre scenariet
5. Kør scenariet

Indsaml det zipfil-output, der skal gives til supportmedarbejderen.
