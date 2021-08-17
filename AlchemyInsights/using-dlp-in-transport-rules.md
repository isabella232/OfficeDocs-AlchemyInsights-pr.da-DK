---
title: Brug af DLP i transportregler
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084088"
---
# <a name="using-dlp-in-transport-rules"></a>Brug af DLP i transportregler

Hvis du vil integrere forebyggelse af datatab (DLP) til en eksisterende transport, skal du bruge betingelsen "**Hvis meddelelsen indeholder...følsomme oplysninger**" i indstillingen Transportregel.

**Du kan finde flere oplysninger i:**

- Integrerede DLP-følsomme oplysningstyper i transportregler: [Integrer regler om følsomme oplysninger](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Du kan også teste reglen med eller uden politiktest ved hjælp af testtilstand på reglen.  Du skal vente 30 minutter, efter at du har oprettet reglen, før du tester den.

- Se [Test regler for mailflow/transport](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Bemærk**: Hvis du forsøger at implementere en ny DLP-politik med transportregler i EAC, kan du bruge [DLP-politikker i sikkerheds- og overholdelsescenter](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stedet.
