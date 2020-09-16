---
title: Fejlfinding af begivenheder fra mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658728"
---
# <a name="troubleshooting-events-from-email"></a>Fejlfinding af begivenheder fra mail

1. Kontrollér, at funktionen er aktiveret for postkassen: **Get-EventsFromEmailConfiguration- <mailbox> Identity**

2. Se derefter på "begivenheder fra mail"-logfilerne **Eksportér-MailboxDiagnosticLogs <mailbox> -komponent TimeProfile**

3. Find den InternetMessageId, der svarer til elementet i postkassen, i "hændelser fra mail"-logfilerne.  

4. TrustScore bestemmer, om elementet er tilføjet eller ej. Hændelser tilføjes kun, hvis TrustScore = "betroet".

TrustScore bestemmes af SPF, DKIM eller dMarc egenskaber, der er i meddelelsens brevhoved.

Sådan får du vist disse egenskaber:

**Skrivebord Outlook**

- Åbne elementet
- File-> egenskaber – > Internet brevhoveder

eller

**MFCMapi**

- Gå til elementet i indbakken
- Søg efter PR_TRANSPORT_MESSAGE_HEADERS_W

Disse egenskaber bestemmes og registreres under transport og routing. Hvis du vil foretage yderligere fejlfinding, skal du muligvis følge med transport support om fejlene i SPF, DKIM og. DMARC.