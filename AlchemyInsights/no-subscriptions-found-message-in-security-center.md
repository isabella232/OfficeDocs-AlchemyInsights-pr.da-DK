---
title: Meddelelse om ingen abonnementer fundet i Sikkerhedscenter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713413"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Meddelelse om ingen abonnementer fundet i Sikkerhedscenter

Hvis du får vist meddelelsen "Der blev ikke fundet nogen abonnementer", mens du åbner Microsoft Defender Security Center, betyder det, at det Azure Active Directory (AAD), der bruges til at logge brugeren på portalen, ikke har en Microsoft Defender ATP-licens.  

Licenserne til Windows E5 og Office E5 er separate licenser.

Åbn en supportsag, hvis licensen blev købt, men ikke er klargjort til denne AAD-forekomst. Enten har du: <br/>
-   Et muligt problem med klargøring af licenser.<br/>
-   Du har utilsigtet klargjort licensen til en anden Microsoft AAD end den, der blev brugt til godkendelse i tjenesten.