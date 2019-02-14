---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964833"
---
# <a name="content-search-not-returning-expected-results"></a>Indhold søgning returnerer ikke forventede resultater

Når du kører søgninger indhold fra Office 365-sikkerhed & Overholdelsescenter, vises der muligvis uventet søgeresultater. Overvej følgende ting, der kan påvirke dine søgeresultater:

- **Indholdssteder og søgebetingelser**: Kontroller, at du har valgt de korrekte indhold placeringer og søgebetingelser. Hvis du har kørt en stor søgning (med mange steder), kan du overveje at opdele det i flere søgninger.

- **Delvist indekserede elementer**: [delvist indekserede elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postkasser er inkluderet i de anslåede søgeresultater. Delvist indekserede elementer fra websteder i SharePoint- og OneDrive medtages dog ikke i estimatet søgning.

- **Søg fejl**: Når du søger efter et stort antal postkasser (mere end 100.000 postkasser), kan du få search-fejl med fejlkoderne som CS008-009- og CS012-002). Prøv i så fald Søg kun efter de mislykkede indholdssteder. Se [denne artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for at få yderligere oplysninger.
