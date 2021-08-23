---
title: Standardetiketindstillingen Outlook ikke anvendt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454568"
---
# <a name="default-outlook-label-setting-not-applied"></a>Standardetiketindstillingen Outlook ikke anvendt

Hvis dine Outlook-standardetiketindstillinger ikke anvendes korrekt, og der ikke er anvendt en anden etiket eller ingen etiket, kan du opleve et kendt problem (MC277818), og du bør gøre en af disse to muligheder for at løse problemet:

**Mulighed 1:**

1. Gå til Microsoft 365 Compliance Center > **Solutions**  >  **Information Protection**.
1. Vælg **Etiketpolitikker**, og vælg den etiketpolitik, du vil redigere (Indstillingen **OutlookDefaultlabel** er ikke angivet korrekt på den pågældende etiketpolitik. Kør **Get-labelpolicy for** at få vist denne indstilling), og vælg derefter **Rediger politik**.
1. Vælg **Næste,** indtil du ser indstillingen Anvend denne standardetiket på **mails,** som er tilgængelig,  hvis du vælger Kræv, at brugerne anvender en etiket på arvingsmails og -dokumenter i dialogboksen Politikindstillinger. 
1. I dialogboksen **Anvend et standardnavn på** dokumenter skal du **vælge** Ingen på rullelisten.
1. Vælg **Næste** og **Send for** at gemme dine etiketindstillinger.

**Mulighed 2:**

I [Security and Compliance Center Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)skal du bruge Set-LabelPolicy commandlet'en til at ændre **OutlookDefaultlabel** til **Ingen** på {OutlookDefaultLabel="None"}.

Kør: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Du kan finde flere oplysninger om standardetiketter Outlook under [Angiv en anden standardetiket til Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).