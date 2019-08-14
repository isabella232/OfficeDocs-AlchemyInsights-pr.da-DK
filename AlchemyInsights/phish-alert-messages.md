---
title: 2491 e-mail-påmindelser fra politikken 'Phish leveres på grund af lejer eller bruger override'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391196"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mail-påmindelser fra politikken 'Phish leveres på grund af lejer eller bruger override'

En standard besked politik med navnet "Phish leveret på grund af lejer eller bruger override" har ført til lejere med Office 365 DTT P1 og P2 licenser. Hvis du har modtaget denne besked, er her de skridt til at undersøge:

1. Fra beskeden, skal du klikke på **Vis besked** for at gå til siden **beskeder** i sikkerhed & Overholdelsescenter.

2. Marker beskeden, du vil se indstillingen til **visning af meddelelseslisten** eller **få vist meddelelser i Explorer**. Begge indstillinger kommer du til detaljerne i e-mailen, der indeholder meddelelsen-ID. Bemærk, at linket trussel Explorer automatisk filtrere meddelelser, der opfylder kriterierne for påmindelser. Du skal muligvis justere Datofilter i Explorer trussel.

Phishing-meddelelsen blev leveret på grund af en tilsidesættelse af manuelt konfigureret:

- En tilladt afsender eller et domæne, der er angivet af brugeren.

- En tilladt afsender eller et domæne, der er angivet af administratoren i en politik om uønskede e-mails.

- Tilladte IP-adresse i en filter forbindelser.

- En mail flow-regel (også kendt som transport), der er konfigureret til at tillade meddelelser i.

Hvis du mener, at meddelelsen blev fejlagtigt markeret som phish, bruge Outlook- [tilføjelsesprogrammet rapporteringsmeddelelse](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) skal forelægge prøver af meddelelsen til Microsoft.
