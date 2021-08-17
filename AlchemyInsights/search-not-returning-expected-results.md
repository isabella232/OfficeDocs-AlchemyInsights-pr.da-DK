---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052704"
---
# <a name="content-search-not-returning-expected-results"></a>Indholdssøgning returnerer ikke de forventede resultater

Når du kører indholdssøgninger fra Microsoft 365 i & overholdelsescenter, modtager du muligvis uventede søgeresultater. Overvej følgende, som kan påvirke dine søgeresultater:

- **Indholdsplaceringer og søgebetingelser:** Sørg for, at du har valgt de korrekte indholdsplaceringer og søgebetingelser. Hvis du har kørt en stor søgning (med mange placeringer), skal du overveje at opdele den i flere søgninger.

- **Delvist indekserede elementer:**  [Delvist indekserede elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra postkasser medtages i de anslåede søgeresultater. Delvist indekserede elementer fra websteder i SharePoint og OneDrive inkluderes dog ikke i det anslåede søgeoverslag.

- **Søgefejl:** Når du søger efter et stort antal postkasser (over 100.000 postkasser), får du muligvis søgefejl med fejlkoder som CS008-009 og CS012-002. I dette tilfælde skal du prøve at søge efter de mislykkede placeringer af indhold igen. Se  [denne artikel for at](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) få flere oplysninger.
