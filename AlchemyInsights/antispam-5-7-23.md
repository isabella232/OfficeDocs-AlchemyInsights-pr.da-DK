---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821405"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Løs problemer med levering af mail, fejlkode 5.7.23

Bekræft SPF DNS-posten for dit domæne på en offentligt tilgængelig SPF- eller DNS-postkontrol på internettet.

Kontrollér, at den udgående meddelelse ikke blev identificeret som spam af Microsoft og dirigeres gennem puljen af levering [med høj risiko.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Meddelelser i pulje til levering af høj risiko består ikke SPF-kontroller og accepteres derfor ikke af destinationens mailorganisation.

Hvis problemet fortsætter, skal du muligvis kontakte administratoren for den mailvært, du forsøger at sende mail til. Læg mærke til de detaljerede eksterne fejl, der er tilgængelige i meddelelsen om ikke-tilgængelig mail. Microsoft Support kan muligvis ikke hjælpe yderligere.
