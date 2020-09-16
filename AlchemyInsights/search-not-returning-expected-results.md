---
title: 1491 – søgning-ikke-returnerede – forventede-resultater
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740468"
---
# <a name="content-search-not-returning-expected-results"></a>Indholdssøgning returnerer ikke forventede resultater

Når du kører indholds søgninger fra Microsoft 365 Security & Compliance Center, får du muligvis uventede søgeresultater. Overvej følgende ting, der kan påvirke søgeresultaterne:

- **Indholds placeringer og søgebetingelser**: Sørg for, at du har valgt de korrekte indholds placeringer og søgebetingelserne. Hvis du har kørt en stor søgning (med mange placeringer), kan du overveje at opdele den i flere søgninger.

- **Delvist indekserede elementer**:  [delvist indekserede elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra postkasser medtages i de anslåede søgeresultater. Delvist indekserede elementer fra websteder i SharePoint og OneDrive medtages dog ikke i søge estimatet.

- **Søgefejl**: når du søger i et stort antal postkasser (over 100.000-postkasser), kan du få søgefejl med fejlkoder som CS008-009 og CS012-002). I dette tilfælde kan du prøve kun at søge efter de mislykkede indholds placeringer. Du kan finde flere oplysninger i  [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
