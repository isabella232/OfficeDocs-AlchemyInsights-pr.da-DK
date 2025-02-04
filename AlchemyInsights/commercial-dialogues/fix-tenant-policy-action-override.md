---
title: Ret lejerpolitik (tilsidesættelse af handling)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326791"
---
# <a name="fix-tenant-policy-action-override"></a>Ret lejerpolitik (tilsidesættelse af handling)

En af dine antispampolitikker har påvirket denne meddelelse. Hvis du vil gennemse politikkerne, skal du gøre følgende:

1. I portalen Microsoft 365 Defender på skal du gå til & politikker for samarbejde & politikker for trussel mod <https://security.microsoft.com/>  \>  \>  \> **uønsket post** i **afsnittet** Politikker.

   For at gå direkte til **siden Politikker for uønsket post** skal du bruge <https://security.microsoft.com/antispam> .

2. På siden Politikker for **uønsket** post skal du vælge politikken ved  at klikke på  navnet på politikken (**Type** er Brugerdefineret politik for uønsket post eller Navn er indgående politik for uønsket post **(standard).**
3. I pop op-menuen med oplysninger, der vises, **skal du vælge Rediger** handlinger i **sektionen** Handlinger.
4. I sektionen  **Meddelelseshandlinger** skal du gennemgå advarslerne for **Spam,** Spam med høj tillid,  **Phishing** og phishing med høj sikkerhed for at se, om nogen af følgende værdier er markeret:
   - **Tilføj X-brevhoved**
   - **Tilføje emnelinje med tekst**
   - **Omdiriger meddelelse til mailadresse**
   - **Slet meddelelse**
   - **Ingen handling**

   Det er muligt, at **standardindstillingerne for alle** brugere Exchange Online Protection påvirkede meddelelsen.

Få mere at vide under [Konfigurer antispam-politikker i EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
