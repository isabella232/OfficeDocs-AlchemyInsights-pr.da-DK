---
title: Service diagnostics tool for Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595515"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service diagnostics tool for Windows Virtual Desktop

WVD (Windows Virtual Desktop) tilbyder et diagnosticeringsværktøj, der gør det muligt for administratorer at identificere fejl via en enkelt grænseflade. Dette værktøj logføres diagnosticeringsrelaterede oplysninger, når WVD bruges af en person, der er tildelt en WVD-rolle. Hver log indeholder oplysninger om den WVD-rolle, der er involveret i aktiviteten, de fejlmeddelelser, der vises under sessionen, og oplysninger om lejeren og brugeren. Azure Log Analytics kan konfigureres til at registrere den aktivitetslog, der er oprettet af diagnosticeringsværktøjet, ved at følge disse trin:

1. Opret et loganalysearbejdsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Forbind Windows-computere til Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Hent arbejdsområde-id'et og den primære nøgle for arbejdsområdet. Konfigurationsguiden skal bruge disse oplysninger for at konfigurere agenten korrekt og for at sikre, at den kan kommunikere med Azure Monitor.

1. [Skubbe diagnosticeringsdata til arbejdsområdet.](https://go.microsoft.com/fwlink/?linkid=2128284) Du kan skubbe diagnostiske data fra din WVD-lejer til Log Analytics for dit arbejdsområde.

1. [Identificer](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) og diagnosticer problemer, der er interne eller eksterne i forhold til WVD.

Hvis du vil have mere at vide om konfiguration af værktøjet til tjenestediagnosticering til WVD, skal du se Brug loganalyse til diagnosticeringsfunktionen.