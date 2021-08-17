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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105346"
---
# <a name="troubleshooting-events-from-email"></a>Fejlfinding af hændelser fra mail

1. Bekræft, at funktionen er aktiveret for **postkassen: Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Kig derefter på "Begivenheder fra **mail"-logfilerne Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. I logfilerne "Begivenheder fra mail" skal du finde det InternetMessageId, der svarer til elementet i postkassen.  

4. TrustScore bestemmer, om elementet tilføjes eller ej. Hændelser tilføjes kun, hvis TrustScore = "Trusted".

TrustScore bestemmes af SPF-, Dkim- eller Dmarc-egenskaberne, som findes i brevhovedet.

Sådan får du vist disse egenskaber:

**Skrivebordsversioner Outlook**

- Åbne elementet
- Egenskaber for filer > -> internetoverskrifter

eller

**MFCMapi**

- Gå til elementet i indbakken
- Se efter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskaber bestemmes og registreres under transport og routing. For yderligere fejlfinding kan det være nødvendigt at følge op med Transport Support vedrørende fejl i SPF, DKIM og.eller DMARC.