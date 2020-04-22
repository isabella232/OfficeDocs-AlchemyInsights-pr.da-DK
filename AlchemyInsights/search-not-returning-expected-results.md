---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709221"
---
# <a name="content-search-not-returning-expected-results"></a>Indholdssøgning returnerer ikke forventede resultater

Når du kører Indholdssøgninger fra Microsoft 365-sikkerhedskontrollen & Overholdelsescenter, modtager du muligvis uventede søgeresultater. Overvej følgende ting, der kan påvirke dine søgeresultater:

- **Indholdsplaceringer og søgebetingelser**: Sørg for, at du har valgt de korrekte indholdsplaceringer og søgebetingelser. Hvis du har kørt en stor søgning (med mange placeringer), kan du overveje at opdele den i flere søgninger.

- **Delvist indekserede elementer**: [Delvist indekserede elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postkasser medtages i de estimerede søgeresultater. Delvist indekserede elementer fra websteder i SharePoint og OneDrive medtages dog ikke i søgeestimatet.

- **Søgefejl**: Når du søger i et stort antal postkasser (over 100.000 postkasser), kan du få søgefejl med fejlkoder som CS008-009 og CS012-002). I dette tilfælde skal du kun prøve at søge efter de fejlbehæftede indholdsplaceringer igen. Se [denne artikel](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for at få flere oplysninger.
