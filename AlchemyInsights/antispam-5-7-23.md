---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682086"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med levering af e-mail for fejlkode 5.7.23

Bekræft SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF-eller DNS-post kontrol på internettet.

Kontroller, at den udgående meddelelse ikke blev identificeret som spam af Office 365, og at den blev distribueret via [puljen med høj risiko](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Meddelelser i den høje risiko leverings pulje vil ikke passere SPF-checks og vil derfor ikke blive accepteret af destinations-e-mail-organisationen.

Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mail vært, som du forsøger at sende mails til. Notér den detaljerede eksterne fejl, der er tilgængelig i meddelelsen Bounce.  Support til Office 365 kan muligvis ikke hjælpe yderligere.