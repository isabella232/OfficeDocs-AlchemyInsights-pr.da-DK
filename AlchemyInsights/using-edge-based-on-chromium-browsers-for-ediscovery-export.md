---
title: Brug af Microsoft Edge baseret på Chromium-browsere til Ediscovery-eksport
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
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834365"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Brug af Microsoft Edge baseret på Chromium-browsere til Ediscovery-eksport

På grund af en nylig ændring vil Microsoft Edge-browsere ikke længere have ClickOnce-understøttelse aktiveret som standard. Hvis du vil fortsætte med at bruge Microsoft 365 eDiscovery-eksportværktøjet, skal du enten bruge Microsoft Internet Explorer eller aktivere ClickOnce-support i Microsoft Edge. 

Sådan aktiverer du ClickOnce-support i Microsoft Edge baseret på Chromium: 
1. I Microsoft Edge-browseren skal du gå til edge://flags/#edge-click-once.
2. For indstillingen ClickOnce-support skal du ændre værdien fra Standard **eller** **Deaktiveret** til **Aktiveret.** 
3. Nederst i browservinduet skal du vælge **Genstart.** <br>
 Ændringen træder i kraft efter genstart af Microsoft Edge. 

Du kan finde oplysninger om dette og trinnene til installation af eksportværktøjet i: [Eksportér resultater fra indholdssøgning.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)