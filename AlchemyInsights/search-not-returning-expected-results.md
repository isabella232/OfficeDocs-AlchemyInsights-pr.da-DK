---
title: 1491-søg-ikke-tilbagevendende-forventede resultater
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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510566"
---
# <a name="content-search-not-returning-expected-results"></a>Indholdssøgning returnerer ikke forventede resultater

Når du kører Indholdssøgninger fra Sikkerhedskontrollen i Microsoft 365 & Compliance Center, modtager du muligvis uventede søgeresultater. Overvej følgende ting, der kan påvirke dine søgeresultater:

- **Indholdsplaceringer og søgebetingelser**: Sørg for, at du har valgt de korrekte indholdsplaceringer og søgebetingelser. Hvis du har foretaget en stor søgning (med mange placeringer), kan du overveje at opdele den i flere søgninger.

- **Delvist indekserede elementer**: [Delvist indekserede elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra postkasser medtages i de estimerede søgeresultater. Delvist indekserede elementer fra websteder i SharePoint og OneDrive medtages dog ikke i søgeestimatet.

- **Søgefejl**: Når du søger i et stort antal postkasser (over 100.000 postkasser), kan du få søgefejl med fejlkoder som CS008-009 og CS012-002). I dette tilfælde skal du kun forsøge at søge efter de mislykkede indholdsplaceringer. Se [denne artikel](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for at få flere oplysninger.
