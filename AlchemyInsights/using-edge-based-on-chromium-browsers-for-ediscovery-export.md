---
title: Brug af Microsoft Edge baseret på Chrombrowsere til eDiscovery-eksport
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
ms.openlocfilehash: d4ccaf4928fb041ec7914b95520c4e7ccdac208c
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741147"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Brug af Microsoft Edge baseret på Chrombrowsere til eDiscovery-eksport

På grund af en nylig ændring vil Microsoft Edge-browserne ikke længere have ClickOnce-understøttelse aktiveret som standard. Hvis du vil fortsætte med at bruge Microsoft Office 365 eDiscovery-eksportværktøjet, skal du enten bruge Microsoft Internet Explorer eller aktivere ClickOnce-understøttelse i Microsoft Edge. 

Sådan aktiveres ClickOnce-understøttelse i Microsoft Edge baseret på chrom: 
1. I din Microsoft Edge-browser, besøg edge://flags/#edge-Klik-én gang.
2. For indstillingen ClickOnce-understøttelse skal du ændre værdien fra **standard** eller **deaktiveret** til **aktiveret**. 
3. Vælg **Genstart**nederst i browservinduet. <br>
 Ændringen træder i kraft efter genstart af Microsoft Edge. 

Oplysninger om dette og trin til installation af eksportværktøjet finder du i: [eksportere søgeresultater for indhold](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).