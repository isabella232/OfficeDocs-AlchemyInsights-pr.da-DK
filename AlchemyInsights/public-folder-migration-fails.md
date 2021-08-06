---
title: Overførsel af offentlige mapper mislykkes ved 95 %
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: e92a983a74ac0b97a613723dacb356ebff68f6cdba2d78ca63085a818d12e739
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923305"
---
# <a name="public-folder-migration-fails-at-95"></a>Overførsel af offentlige mapper mislykkes ved 95 %

Du har muligvis startet fuldførelsen af en overførselsbatch, og status **for** overførselsbatchen fortsætter med at vise Synkroniseret i meget lang tid. Dette er den forventede funktionsmåde.

Det er normalt, at status for en overførselsbatch forbliver på Synkroniseret **i** et par timer, før den skifter til **Fuldførelse**. For migrering med et stort antal målpostkasser er det normalt at se statussen forblive i den synkroniserede tilstand i mere end 24 timer, hvis ingen af de underliggende offentlige mappeoverførselsanmodninger mislykkedes eller var i karantæne. Der kan gå 24-48 timer, før overførselsbatchen er fuldført.

For overførsel af offentlige mapper mislykkes ved 95 %, med fejlen FailedToMailEnablePublicFoldersException:

1. Download og kør [scriptet ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) på din Exchange lokale server.

2. Udfør de afhjælpende handlinger, der foreslås af scriptet.

3. Kør Sync-MailPublicFolders (i Exchange 2010) eller Sync-ModernMailPublicFolders (for Exchange 2013 og nyere).

4. Genoptag overførsel af offentlig mappe.
