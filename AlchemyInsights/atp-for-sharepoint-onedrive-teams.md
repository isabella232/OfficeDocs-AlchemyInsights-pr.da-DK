---
title: Microsoft Defender til Office 365 til SharePoint, OneDrive og Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: c42786559d527a5ef9a0a8cfad1476f4d122b6d5570ca5b9ea138b21a153ae96
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896329"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender til Office 365 til SharePoint, OneDrive og Microsoft Teams

Følg disse trin for at aktivere Microsoft Defender for Office 365:

1. Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator- eller sikkerhedsadministratorkonto.

2. I venstre navigationsrude under **Trusselsstyring skal** du **vælge Politik Pengeskab** \> **Vedhæftede filer**.

3. Vælg **Slå Defender til for Office 365 for SharePoint, OneDrive og Microsoft Teams**.

4. [Opret en politik for aktivitetsbeskeder](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) for at modtage meddelelser, når vi registrerer skadelige filer.

Du kan finde en komplet vejledning [i denne Aktiver Pengeskab Vedhæftede filer for SharePoint, OneDrive og Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)

**Bemærk!** Som designet scanner Microsoft Defender Office 365 ikke hver enkelt fil i SharePoint Online, OneDrive for Business eller Microsoft Teams. Filer scannes asynkront af en proces, der bruger delingsaktivitet, gæsteaktivitet og trusselssignaler til at identificere skadelige filer. Du kan finde flere [oplysninger Pengeskab Vedhæftede filer til SharePoint, OneDrive og Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
