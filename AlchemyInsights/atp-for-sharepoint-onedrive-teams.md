---
title: DTT for SharePoint, OneDrive og Microsoft-Team
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764948"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>DTT for SharePoint, OneDrive og Microsoft-Team

Følg disse trin for at aktivere avanceret Threat Protection:

1. Gå til [https://protection.office.com](https://protection.office.com) og logge på med en global administrator eller sikkerhedsadministratorkonto.

2. Vælg **politik** i den venstre navigationsrude under **Administration af truslen**, \> **Sikre vedhæftede filer**.

3. Vælg **Slå DTT for SharePoint, OneDrive, og Microsoft-Team**.

4. [Oprette en aktivitet besked politik](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) til at modtage besked, når vi registrere skadelige filer.

Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Bemærk**: ved design, ATP ikke scanne hver enkelt fil i SharePoint Online, OneDrive til arbejde eller Microsoft-Teams. Filer scannes asynkront ved en proces, der bruger Deling aktivitet, aktivitet for gæst, og truslen signaler til at identificere skadelige filer. Yderligere oplysninger finder du i dette [emne](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
