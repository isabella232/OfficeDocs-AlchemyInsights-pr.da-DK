---
title: Fejlfinding af hændelser fra mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569007"
---
# <a name="troubleshooting-events-from-email"></a>Fejlfinding af hændelser fra mail

1. Kontroller, at funktionen er aktiveret for postkassen: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Så kig på 'Begivenheder fra e-mail' logger **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Find det InternetMessageId, der svarer til elementet i postkassen, i logfilerne 'Hændelser fra e-mail'.  

4. TrustScore bestemmer, om varen tilføjes eller ej. Hændelser tilføjes kun, hvis TrustScore = "Trusted".

TrustScore bestemmes af egenskaberne SPF, Dkim eller Dmarc, som findes i brevhovedet.

Sådan får du vist disse egenskaber:

**Outlook på computeren**

- Åbne elementet
- Egenskaber for fil -> -> Internetheads

Eller

**MFCMapi delte et eller flere**

- Gå til elementet i indbakken
- Kig efter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskaber bestemmes og registreres under transport og ruteføring. For yderligere fejlfinding kan det være nødvendigt at følge op med Transport Support om fejl i SPF, DKIM og.eller DMARC.