---
title: Overførsel af offentlige mapper mislykkes ved 95%
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
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47803493"
---
# <a name="public-folder-migration-fails-at-95"></a>Overførsel af offentlige mapper mislykkes ved 95%

Du har muligvis indledt fuldførelsen af en overførselsbatch, og status for overførsels batchen fortsætter med at blive **synkroniseret** i meget lang tid. Dette er den forventede funktionsmåde.

Det er almindeligt for en overførsels batchs status at forblive **synkroniseret** for et par timer, før den skifter til **fuldførelse**. For overførsler, der omfatter et stort antal destinations postkasser, er det normalt at se status forbliver i synkroniseret tilstand i mere end 24 timer, forudsat at ingen af de underliggende anmodninger om overførsel af offentlige mapper mislykkedes eller var i karantæne. Tillad 24-48 timer for overførsels batchen for at fuldføre opgaverne.

For overførsler af offentlige mapper, der mislykkedes på 95%, med fejl FailedToMailEnablePublicFoldersException:

1. Download og Kør [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) -scriptet på din Exchange-Server i det lokale miljø.

2. Udføre de rette handlinger, der foreslås af scriptet.

3. Kør Sync-MailPublicFolders (for Exchange 2010) eller sync-ModernMailPublicFolders (for Exchange 2013 og nyere).

4. Genoptag overførsel af offentlige mapper.
