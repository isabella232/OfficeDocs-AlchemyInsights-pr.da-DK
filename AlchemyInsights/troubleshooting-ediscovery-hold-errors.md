---
title: Fejlfinding af ediscovery indeholder fejl
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676084"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Fejlfinding af ediscovery indeholder fejl

Oplever du problemer med eDiscovery-ventende emner? Her er nogle af de bedste fremgangsmåder at overveje:

- Kontrollér status for ventepositionsfordelingen.  Hvis status er **Til (Afventer)** eller **Fra (Afventer),** skal du vente på, at ventepositionsfordelingen fuldføres.
- Flet opdateringer af eDiscovery-venteposition til en enkelt anmodning om flere poster i stedet for at opdatere politikken gentagne gange for hver transaktion.
- Kør Set-CaseHoldPolicy <policyname> -RetryDistribution i Security and Compliance Center Powershell. Du kan finde flere [oplysninger Forbind Security & Compliance Center PowerShell.](/powershell/exchange/connect-to-scc-powershell)

Du kan finde trin til at kontrollere disse indstillinger og yderligere bedste fremgangsmåder for at mindske og løse problemer med ventepositioner i eDiscovery under Fejlfinding af [eDiscovery-ventepositionsfejl.](/microsoft-365/compliance/hold-distribution-errors)
Du kan finde oplysninger om fejlfinding af andre almindelige eDiscovery-problemer under Undersøge, foretage [fejlfinding og løse almindelige eDiscovery-problemer.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
