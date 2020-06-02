---
title: ATP til SharePoint-, OneDrive- og Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508406"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP til SharePoint-, OneDrive- og Microsoft Teams

Følg disse trin for at aktivere avanceret trusselsbeskyttelse:

1. Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator- eller sikkerhedsadministratorkonto.

2. Vælg Vedhæftede filer, der er tillid til, **i** venstre navigationsrude under **Trusselsstyring** \> **Safe Attachments**.

3. Vælg **Slå ATP til for SharePoint, OneDrive og Microsoft Teams**.

4. [Opret en politik for aktivitetsbesked](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) for at modtage meddelelser, når vi registrerer skadelige filer.

Du kan finde flere instruktioner i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Bemærk:** Efter design scanner ATP ikke hver enkelt fil i SharePoint Online, OneDrive for Business eller Microsoft Teams. Filer scannes asynkront af en proces, der bruger delingsaktivitet, gæsteaktivitet og trusselssignaler til at identificere skadelige filer. Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
