---
title: ATP til SharePoint, OneDrive og Microsoft Teams
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
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712452"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP til SharePoint, OneDrive og Microsoft Teams

Følg disse trin for at aktivere Avanceret trusselsbeskyttelse:

1. Gå [https://protection.office.com](https://protection.office.com) til og log på med en global administrator- eller sikkerhedsadministratorkonto.

2. Vælg **Politiksikre** \> vedhæftede filer i venstre navigationsrude under **Trusselsstyring**. **Safe Attachments**

3. Vælg **Slå ATP til for SharePoint, OneDrive og Microsoft Teams**.

4. [Opret en politik](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) for aktivitetsadvarsler for at modtage meddelelser, når vi registrerer skadelige filer.

Du kan finde komplette instruktioner i dette [emne](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Bemærk:** Efter design scanner ATP ikke hver eneste fil i SharePoint Online, OneDrive for Business eller Microsoft Teams. Filer scannes asynkront af en proces, der bruger delingsaktivitet, gæsteaktivitet og trusselssignaler til at identificere ondsindede filer. Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
