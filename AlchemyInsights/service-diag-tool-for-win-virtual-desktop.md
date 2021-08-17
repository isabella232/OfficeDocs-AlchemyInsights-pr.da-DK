---
title: Service diagnostics tool for Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052380"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Service diagnostics tool for Windows Virtual Desktop

Windows Virtual Desktop (WVD) tilbyder et diagnosticeringsværktøj, der gør det muligt for administratorer at identificere fejl via en enkelt grænseflade. Dette værktøj logføres diagnosticeringsrelaterede oplysninger, når WVD bruges af en person, der er tildelt en WVD-rolle. Hver log indeholder oplysninger om den WVD-rolle, der er involveret i aktiviteten, de fejlmeddelelser, der vises under sessionen, og oplysninger om lejeren og brugeren. Azure Log Analytics kan konfigureres til at registrere den aktivitetslog, der er oprettet af diagnosticeringsværktøjet. Sådan gør du:

1. Opret et Log Analytics-arbejdsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) [eller Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Forbind Windows computere til Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Få arbejdsområde-id'et og den primære nøgle for dit arbejdsområde. Konfigurationsguiden skal bruge disse oplysninger for at konfigurere agenten korrekt og for at sikre, at den kan kommunikere med Azure Monitor.
1. [Skubbe diagnosticeringsdata til dit arbejdsområde.](https://go.microsoft.com/fwlink/?linkid=2128284) Du kan skubbe diagnostiske data fra din WVD-lejer til LogAnalyse for dit arbejdsområde.
1. [Identificer og diagnosticer](https://go.microsoft.com/fwlink/?linkid=2128338) problemer, der er interne eller eksterne i forhold til WVD.

Hvis du vil have mere at vide om konfiguration af tjenestediagnosticeringsværktøjet til WVD, skal du se Brug [loganalyse til diagnosticeringsfunktionen.](https://go.microsoft.com/fwlink/?linkid=2128084)
