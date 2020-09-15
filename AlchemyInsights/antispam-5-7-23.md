---
title: Spam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717319"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med levering af mail for fejlkode 5.7.23

Kontrollér SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF-eller DNS-post kontrol på internettet.

Kontrollér, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og sendt via [puljen til stor risiko levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Meddelelser i puljen til levering af høj risiko opfylder ikke SPF checks, og de accepteres derfor ikke af organisationens destinations-e-mail.

Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mail vært, du forsøger at sende mail til. Vær opmærksom på den detaljerede eksterne fejl, der er tilgængelig i meddelelsen bold. Microsoft Support kan muligvis ikke hjælpe yderligere.
