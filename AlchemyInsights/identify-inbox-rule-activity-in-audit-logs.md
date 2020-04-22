---
title: Identificer aktivitet for indbakkeregel i overvågningslogfiler
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716418"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificer aktivitet for indbakkeregel i overvågningslogfiler

Du kan bruge overvågningslogsøgning i Microsoft 365 Security & Compliance Center til at få vist regelhændelser i indbakken (oprettelse, ændring og sletning af indbakkeregler).

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til**søgesiden for søgefilen til søgeovervågning** i **søgefilen** > til søgning i søgeområdet.

3. Vælg datointervallet i felterne **Startdato** **og Slutdato.**

4. Under **Exchange Mailbox Activities**skal du kontrollere , at feltet **Aktiviteter** er angivet til **Ny IndbakkeRegel Opret/rediger/aktiver/deaktiver indbakkereglen**.

5. Klik på **Søg**.

Vælg en overvågningspost i resultaterne. Klik på Flere oplysninger i pop **op-vinduet med**detaljer . Oplysninger om indstillingerne for indbakkeregel vises i feltet **Parametre.**

Du kan finde flere oplysninger [under Bestemme, om en bruger har oprettet en indbakkeregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
