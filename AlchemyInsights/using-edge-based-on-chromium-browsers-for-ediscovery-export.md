---
title: Brug af Microsoft Edge baseret på Chrom-browsere til ediscovery-eksport
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 5c247ab69c272d2d296f9602fc5246a08164da5e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726206"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Brug af Microsoft Edge baseret på Chrom-browsere til ediscovery-eksport

På grund af en nylig ændring, vil Microsoft Edge browsere ikke længere have ClickOnce support aktiveret som standard. Hvis du vil fortsætte med at bruge Microsoft 365 eDiscovery Export Tool, skal du enten bruge Microsoft Internet Explorer eller aktivere ClickOnce-support i Microsoft Edge. 

Sådan aktiveres ClickOnce-understøttelse i Microsoft Edge baseret på Chrom: 
1. Besøg edge://flags/#edge-click-once i din Microsoft Edge-browser.
2. For indstillingen ClickOnce Support skal du ændre værdien fra **Standard** eller **Deaktiveret** til **Aktiveret**. 
3. Vælg **Genstart**nederst i browservinduet. <br>
 Ændringen træder i kraft, når Microsoft Edge er genstartet. 

Du kan finde oplysninger om dette og trin til installation af eksportværktøjet under: [Eksportere søgeresultater for indhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).