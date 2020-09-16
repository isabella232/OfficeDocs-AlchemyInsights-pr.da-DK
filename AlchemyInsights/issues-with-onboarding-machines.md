---
title: Problemer med Onboarding-maskiner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676876"
---
# <a name="issues-with-onboarding-machines"></a>Problemer med Onboarding-maskiner

Der kan være problemer med Onboarding af computere til MDATP-tjenesten. Hvis du har adgang til slutbrugerens maskine, skal du følge disse trin:

1. Hent diagnosticeringsværktøjet til [klient forbindelses analyse](https://aka.ms/mdatpanalyzer) .
2. Udpak og Kør MDATPAnalyzer. cmd.
3. Find diagnosticeringslogfilen i den mappe, der hedder MDATPClientAnalyzerResult, den samme mappe, hvor Analyseværktøjet er hentet.
4. Gennemse logfilen, MDATPClientAnalyzer.txt, for at finde problemer med forbindelse eller Internet proxyindstillinger.