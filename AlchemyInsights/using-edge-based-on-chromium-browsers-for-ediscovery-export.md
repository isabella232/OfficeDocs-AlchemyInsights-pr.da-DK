---
title: Brug Microsoft Edge baseret på Chromium til Ediscovery-eksport
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: a583896b5aa8e73be5e932a729c380acc8092e73b2151647c999f9a7b69669b6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998382"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Brug Microsoft Edge baseret på Chromium til Ediscovery-eksport

På grund af en nylig ændring Microsoft Edge browsere ikke længere understøttes ClickOnce understøttet som standard. Hvis du vil fortsætte med at bruge Microsoft 365 eDiscovery-eksportværktøjet, skal du enten bruge Microsoft Internet Explorer eller aktivere ClickOnce-support i Microsoft Edge. 

Sådan aktiveres ClickOnce support i Microsoft Edge baseret på Chromium: 
1. I din Microsoft Edge skal du gå til edge://flags/#edge-click-once.
2. For at ClickOnce support skal du ændre værdien fra Standard **eller** **Deaktiveret til** **Aktiveret.** 
3. Nederst i browservinduet skal du vælge **Genstart.** <br>
 Ændringen træder i kraft efter genstart Microsoft Edge. 

Du kan finde oplysninger om dette og trinnene til installation af eksportværktøjet i: [Eksportér resultater fra indholdssøgning.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)