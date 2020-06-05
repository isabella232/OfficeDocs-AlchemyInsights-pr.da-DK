---
title: Manglende e-mails i karantæne
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569046"
---
# <a name="missing-emails-in-quarantine"></a>Manglende e-mails i karantæne"

Administratorer kan [få vist, frigive eller slette disse meddelelser.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Hvis du vil åbne Sikkerheds- & Compliance Center, skal du gå til [https://protection.office.com](https://protection.office.com/) . Hvis du vil åbne siden Karantæne direkte, skal du gå til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Du kan søge efter følgende værdier:  

- **Meddelelses-id**: Meddelelsens globalt entydige id. Hvis du vælger en meddelelse på listen, vises værdien **for meddelelses-id** i pop op-vinduet **Detaljer.** Administratorer kan bruge [meddelelsessporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til at finde meddelelser og deres tilsvarende værdier for meddelelses-id.
- **Afsenders e-mailadresse**: En enkelt afsenders e-mailadresse.
- **Modtagers e-mailadresse**: En enkelt modtagers e-mailadresse.
- **Emne**: Brug hele meddelelsens emne. Der skelnes ikke mellem store og små bogstaver i søgningen.

Når du har angivet søgekriterierne, skal du klikke på ![ Knappen ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Opdater** for at filtrere resultaterne.  

De cmdletter, du bruger til at få vist og administrere meddelelser og filer i karantæne, er:
- [Slet-karantæneMeddelelse](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksport-KarantæneMeddelelse](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Bliv karantæneMeddelelse](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Eksempel-karantæneMeddelelse](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bemærk, at denne cmdlet kun er til meddelelser, ikke malwarefiler fra ATP til SharePoint Online, OneDrive for Business eller Teams.
- [Release-KarantæneMeddelelse](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)