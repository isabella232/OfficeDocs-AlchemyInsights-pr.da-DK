---
title: Fejlfinding af hændelser fra mail
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834833"
---
# <a name="troubleshooting-events-from-email"></a>Fejlfinding af hændelser fra mail

1. Bekræft, at funktionen er aktiveret for **postkassen: Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Kig derefter på "Begivenheder fra **mail"-logfilerne Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. I logfilerne "Begivenheder fra mail" skal du finde det InternetMessageId, der svarer til elementet i postkassen.  

4. TrustScore bestemmer, om elementet tilføjes eller ej. Hændelser tilføjes kun, hvis TrustScore = "Trusted".

TrustScore bestemmes af SPF-, Dkim- eller Dmarc-egenskaberne, som findes i brevhovedet.

Sådan får du vist disse egenskaber:

**Skrivebordsversionen af Outlook**

- Åbne elementet
- Egenskaber for filer > -> internetoverskrifter

eller

**MFCMapi**

- Gå til elementet i indbakken
- Se efter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskaber bestemmes og registreres under transport og routing. For yderligere fejlfinding kan det være nødvendigt at følge op med Transport Support vedrørende fejl i SPF, DKIM og.eller DMARC.