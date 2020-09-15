---
title: DTT til SharePoint, OneDrive og Microsoft teams
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715555"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>DTT til SharePoint, OneDrive og Microsoft teams

Følg disse trin for at aktivere avanceret trusselsbeskyttelse:

1. Gå til [https://protection.office.com](https://protection.office.com) og log på med en global administrator-eller sikkerhedsadministrator konto.

2. Vælg **politik** sikre vedhæftede filer i venstre navigationsrude under **trussels administration** \> **Safe Attachments**.

3. Vælg **Aktivér DTT for SharePoint, OneDrive og Microsoft teams**.

4. [Opret en politik for besked om aktivitet](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) for at modtage meddelelser, når vi registrerer ondsindede filer.

Du kan finde en komplet vejledning i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Bemærk**: efter design scanner DTT ikke alle enkeltfiler i SharePoint Online, OneDrive for Business eller Microsoft teams. Filer scannes asynkront af en proces, der bruger delings aktivitet, gæste aktivitet og trusler signaler til at identificere ondsindede filer. Du kan finde flere oplysninger i dette [emne](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
