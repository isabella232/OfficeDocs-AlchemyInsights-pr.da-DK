---
title: Brug af DLP i transportregler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915090"
---
# <a name="using-dlp-in-transport-rules"></a>Brug af DLP i transportregler

Hvis du vil integrere forebyggelse af datatab (DLP) til en eksisterende transport, skal du bruge betingelsen "**Hvis meddelelsen indeholder...følsomme oplysninger**" i indstillingen Transportregel.

**Du kan finde flere oplysninger i:**

- Integrerede DLP-følsomme oplysningstyper i transportregler: [Integrer regler om følsomme oplysninger](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Du kan også teste reglen med eller uden politiktest ved hjælp af testtilstand på reglen.  Du skal vente 30 minutter, efter at du har oprettet reglen, før du tester den.

- Se [Test regler for mailflow/transport](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Bemærk**: Hvis du forsøger at implementere en ny DLP-politik med transportregler i EAC, kan du bruge [DLP-politikker i sikkerheds- og overholdelsescenter](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stedet.
