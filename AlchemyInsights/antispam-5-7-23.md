---
title: Antispam - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676491"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med levering af mail, fejlkode 5.7.23

Kontroller SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF- eller DNS-postkontrol på internettet.

Kontroller, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og dirigeret gennem [puljen til levering med høj risiko](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Meddelelser i puljen til levering af høj risiko består ikke SPF-checks og accepteres derfor ikke af destinationsmailorganisationen.

Hvis problemet fortsætter, skal du muligvis kontakte administratoren af den mailvært, du forsøger at sende e-mail til. Noter den detaljerede eksterne fejl, der er tilgængelig i afvisningsmeddelelsen. Microsoft-support kan muligvis ikke hjælpe yderligere.
