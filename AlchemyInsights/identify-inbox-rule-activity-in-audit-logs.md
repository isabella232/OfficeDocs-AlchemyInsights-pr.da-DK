---
title: Identificere aktivitet for Indbakke regel i overvågningslogge
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779045"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificere aktivitet for Indbakke regel i overvågningslogge

Du kan bruge søgning i overvågningsloggen i Microsoft 365 Security & overholdelses Center til at få vist regler for Indbakke-regler (oprette, redigere og slette indbakkeregler).

1. Log på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).

2. Gå til søgesiden **Søg i**  >  **overvågningslogfil** .

3. Vælg datointervallet i felterne **Start dato** og **Slutdato** .

4. Under **aktiviteter for Exchange-postkassen**skal du kontrollere, at feltet **aktiviteter** er indstillet til **New-InboxRule Create/Modify/enable/disable indbakke Rule**.

5. Klik på **Søg**.

I resultaterne skal du vælge en revisionspost. Klik på **flere oplysninger**i pop op-vinduet detaljer. Oplysninger om indstillingerne for Indbakke-reglen vises i feltet **parametre** .

Du kan finde flere oplysninger under [afgøre, om en bruger har oprettet en indbakke regel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
