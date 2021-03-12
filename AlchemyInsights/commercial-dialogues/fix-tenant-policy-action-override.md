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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744479"
---
# <a name="fix-tenant-policy-action-override"></a>Ret lejerpolitik (tilsidesættelse af handling)

En antispampolitik i din lejer har påvirket denne meddelelse. Hvis du vil gennemse politikken, skal du gøre følgende:

1. Gå til [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)og gå derefter til antispam **for**  >    >  [politikker for trusselsadministration.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Kontrollér, om  politikkilden angiver følgende: Meddelelsen **Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC**

    Hvis det er ja, skal **du under** fanen Brugerdefineret kontrollere indstillingerne for den politik, der har påvirket meddelelsen. Det er muligt, at standardindstillingerne **for alle** Exchange Online Protection-kunder påvirkede meddelelsen.

Du kan finde flere oplysninger om konfiguration af politikker for spamfilter i [Konfigurere politikker for spamfiltrering.](https://go.microsoft.com/fwlink/?linkid=2101431)
