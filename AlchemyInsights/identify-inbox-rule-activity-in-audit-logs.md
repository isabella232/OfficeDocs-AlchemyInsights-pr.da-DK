---
title: Identificere Indbakke regel aktivitet i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539156"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificere Indbakke regel aktivitet i overvågningslogge

Du kan bruge overvågning log søgning i Office 365 sikkerhed & Overholdelsescenter Indbakke regel hændelser (oprettelse, ændring og sletning af regler for Indbakke).

1. Log på [Office 365 sikkerhed & Overholdelsescenter](https://protection.office.com/).

2. Gå til **Søg** > **revision log** søgeside.

3. Vælg datointervallet i felterne **startdato** og **slutdato** .

4. Under **Exchange postkasse aktiviteter**, skal du kontrollere feltet **aktiviteter** er indstillet til **Ny InboxRule Opret/Rediger/aktivere/deaktivere indbakkeregel**.

5. Klik på **Søg**.

Vælg en revisionspost i resultaterne. Oplysninger om mærke, klik på **Flere oplysninger**. Oplysninger om indstillinger for regler i Indbakke vises i feltet **parametre** .

Yderligere oplysninger finder du [fastlægge, hvis en bruger har oprettet en regel for Indbakke](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
