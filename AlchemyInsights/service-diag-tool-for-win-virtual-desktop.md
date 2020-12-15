---
title: Værktøjet tjeneste diagnosticering til Windows virtuelt skrivebord
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677649"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Værktøjet tjeneste diagnosticering til Windows virtuelt skrivebord

Windows virtuelt skrivebord (WVD) tilbyder et diagnosticeringsværktøj, der gør det muligt for administratorer at identificere fejl via en enkelt grænseflade. Dette værktøj registrerer diagnosticerings relaterede oplysninger, når WVD bruges af en person, der har fået tildelt en WVD-rolle. Hver log indeholder oplysninger om den WVD-rolle, der er involveret i aktiviteten, de fejlmeddelelser, der vises under sessionen, og oplysningerne om lejeren og brugeren. Azure log Analytics kan konfigureres til at registrere aktivitetslogfilen, der er oprettet af værktøjet diagnosticering. Sådan gør du:

1. Oprette et log Analytics-arbejdsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Oprette forbindelse mellem Windows-computere og Azure-skærm](https://go.microsoft.com/fwlink/?linkid=2129913). Hent arbejdsområde-id'et og den primære nøgle i dit arbejdsområde. Konfigurationsguiden skal have disse oplysninger for at konfigurere agenten korrekt og sikre, at den kan kommunikere med Azure Monitor.
1. [Overfør diagnosticeringsdata til arbejdsområdet](https://go.microsoft.com/fwlink/?linkid=2128284). Du kan skubbe diagnosticeringsdata fra din WVD-lejer til en logfils analyse for dit arbejdsområde.
1. [Identificer og Diagnosticer problemer](https://go.microsoft.com/fwlink/?linkid=2128338) , der er interne eller eksterne i forhold til WVD.

Hvis du vil have mere at vide om konfiguration af værktøjet til tjeneste diagnosticering for WVD, skal du se [brug af log analyse til diagnosticerings funktionen](https://go.microsoft.com/fwlink/?linkid=2128084).
