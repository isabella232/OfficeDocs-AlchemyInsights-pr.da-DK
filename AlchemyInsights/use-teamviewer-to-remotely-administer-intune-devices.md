---
title: Brug TeamViewer til fjernadministrering af Intune-enheder
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554841"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Brug TeamViewer til fjernadministrering af Intune-enheder

Enheder, der administreres af Intune, kan fjernadministreres ved hjælp [af TeamViewer](https://www.teamviewer.com/).

Hvis du vil administrere Intune ved hjælp af TeamViewer, skal du følge disse trin: 

Begynd med at indhente legitimationsoplysninger fra TeamViewer for at konfigurere TeamViewer Connector på Intune. Dette gør det muligt for administratoren at angive legitimationsoplysninger i TeamViewer Connector-brugergrænsefladen under Enheder, en engangshandling for at oprette forbindelsen mellem Intune og TeamViewer-tjenesten.

**Del 1: Start en session med en ekstern enhed**

1. Vælg **den enhed**, du vil starte en fjernsession med, under Alle enheder .
2. Fra **... Mere**, vælg **Ny fjernsupportsession**.
3. Vælg **Ja for** at bekræfte, at du vil oprette en fjernsession.
    Når anmodningen "Igangsættelse af en ny fjernsession" er bekræftet af TeamViewer-tjenesten, får du vist en mulighed for **at starte fjernsupport** under oplysningerne i ruden Oversigt (eller Essentials) for enheden. Vælg **Se mere** for at udvide ruden og få vist status for Fjernsupport.
4. Vælg **Start fjernsession** for at starte sessionen på administratorsiden.
5. Vælg at hente den binære TeamViewer (Windows), og vælg **Kør**.<br/>
    **Bemærk:** Du kan ignorere enhver webbrowserside, der er åbnet på TeamViewer-webstedet.

6. Bekræft anmodningen om, at TeamViewer-appen skal foretage ændringer på enheden (kun Windows).
7. TeamViewer-appen starter og indeholder sessionskoden for at godkende forbindelsen til fjernenheden.

**Del 2: På den enhed, der er målrettet til en fjernsession**

1. Åbn Intune-firmaportalen.
2. Se efter et meddelelsesflag: "It-administratoren anmoder om kontrol af denne enhed til en fjernsupportsession", og vælg meddelelsen.
3. Vælg at downloade TeamViewer-programmet, eller bekræft download af TeamViewer-appen fra App Store, og vælg **Kør**.
    **Bemærk:** Du kan ignorere enhver webbrowserside, der er åbnet på TeamViewer-webstedet.

4. Bekræft anmodningen om, at TeamViewer-appen skal foretage ændringer på enheden (kun Windows).
5. TeamViewer-appen starter og indeholder sessionskoden for at godkende forbindelsen til fjernenheden.
6. Et pop op-vindue bliver spurgt, om du vil tillade, at sessionen starter.

**Bemærk:** De sessionskoder, der genereres af TeamViewer-tjenesten, bruges kun én gang. Hvis du mister forbindelsen, skal du:

1. Luk forekomsten af TeamViewer-appen på fjernenheden og på administratorarbejdsstationen.
2. Luk firmaportalen på fjernenheden.
3. Start en ny "Ny fjernsupportsession" fra administrationsportalen.
4. Åbn firmaportalen på fjernenheden igen for at modtage den nye meddelelse.
5. Download og åbn TeamViewer-appen på både fjernenheden og administratorarbejdsstationen som før.