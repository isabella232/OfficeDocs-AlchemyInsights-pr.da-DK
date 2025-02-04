---
title: Løs almindelige problemer med Microsoft Defender til Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330054"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Løs almindelige problemer med Microsoft Defender til Office 365

Her er nogle løsninger på almindelige problemer med Microsoft Defender til Office 365:

- **Meddelelsesforsinkelse:**

  Forsinkelser i levering af mail kan være årsag til Pengeskab scanning af vedhæftede filer i meddelelser. Du kan finde flere oplysninger [Pengeskab indstillinger for politik for vedhæftede filer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Rapportere falske positive eller negative resultater:**

  Få mere at vide under [Rapportér meddelelser og filer til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Aktivér Pengeskab Link-beskyttelse:**

  1. I Microsoft 365 Defender på skal du gå til & politikker for samarbejde & politikker for Pengeskab regler og Pengeskab <https://security.microsoft.com/>  \>  \>  \>  **i sektionen** Politikker.

     For at gå direkte til **siden Pengeskab Links skal** du bruge <https://security.microsoft.com/safelinksv2> .

  2. På siden **Pengeskab links** skal du vælge politikken ved at klikke på navnet på politikken.
  3. I pop op-vindue med oplysninger, der vises, skal du gøre et af følgende:
     - Hvis du vil tilføje en ny politik, skal du **vælge + Opret.** Der starter en guide, der kan hjælpe dig med at definere dine politikindstillinger.
     - Hvis du vil redigere en eksisterende politik, skal du vælge politikken ved at klikke på navnet på politikken. I pop op-menuen med oplysninger, der vises, **skal du** vælge Rediger i **sektionen Beskyttelsesindstillinger.**
  4. På siden **Beskyttelse skal** du konfigurere følgende indstillinger:
     - Slå Vælg **handlingen for ukendte potentielt skadelige URL-adresser i meddelelser til.**
     - Vælg **Anvend sikre links til meddelelser, der er sendt i organisationen.**

  Du kan finde flere oplysninger [i Konfigurere Pengeskab Links-politikker i Microsoft Defender til Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
