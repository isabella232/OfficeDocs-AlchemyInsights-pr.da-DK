---
title: Identificer aktivitet for indbakkeregel i overvågningslogfiler
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
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891289"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificer aktivitet for indbakkeregel i overvågningslogfiler

Du kan bruge søgning i overvågningsloggen i Microsoft 365 Overholdelsescenter til at få vist indbakkeregelhændelser (oprettelse, ændring og sletning af indbakkeregler).

1. Gør et af følgende:
   - I Microsoft 365 Overholdelsescenter på <https://compliance.microsoft.com> skal du gå til **Løsningsrevision** \> . Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://compliance.microsoft.com/auditlogsearch> .
   - I portalen Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Overvågning**. Du kan også gå direkte til siden **Overvågning ved** hjælp af <https://security.microsoft.com/auditlogsearch> .

2. På fanen **Søg** på siden **Overvågning** skal du konfigurere følgende indstillinger:
   - **Dato- og tidsinterval:** Markér dato/klokkeslæt-området i **felterne Start** **og** Slut.
   - **Aktiviteter:** Vælg en eller flere af følgende værdier:
     - **Ny indbakkeregel Opret indbakkeregel ud fra Outlook Web App**
     - **Angiv IndbakkeRegel Rediger regel fra Outlook Web App**.
     - **Opdatere indbakkeregler fra Outlook klient**

3. Når du er færdig, skal du klikke på **Søg**. Aktiviteterne vises på den nye **overvågningssøgningsside.**

4. Vælg en aktivitet i resultaterne for at åbne pop op-dialogboksen med detaljer. Oplysninger om indstillinger for indbakkeregel vises i **feltet** Parametre.

Du kan finde flere oplysninger under [Fastslå, om en bruger har oprettet en indbakkeregel](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
