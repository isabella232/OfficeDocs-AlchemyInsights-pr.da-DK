---
title: Kommentarer til listeelementer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982453"
---
# <a name="comments-on-list-items"></a>Kommentarer til listeelementer

Brugerne vil snart kunne tilføje og slette kommentarer til listeelementer. Brugere kan se alle kommentarer på et listeelement og filtrere mellem visninger, der viser kommentarer eller aktiviteter relateret til et element.

**Tidsindstilling** :

**Målrettet udgivelse** : gradvis rulning i midten af oktober og forventes at blive gennemført i midten-november

**Standard version** : gradvis rulning i midt-november og forventes at blive afsluttet i starten af december

**Udrulning** : målrettet udgivelse for hele organisationen

Brugerne skal bemærke følgende, før de kan tilføje og slette kommentarer:

- Kommentarer følger de tilladelsesindstillinger, der er indbygget i SharePoint.
- Klassiske lister, der endnu ikke er bygget til at blive vist i moderne brugergrænseflader, f. eks. opgavelister, vil ikke have denne kommentarfunktion.
- Kommentering på lister i teams er ikke tilgængelig med denne version.
- Kommentarer indekseres ikke ved søgning.

Administratorer kan deaktivere denne funktion på organisationsniveau ved at ændre **CommentsOnListItemsDisabled** -parameteren i cmdlet'en **set-SPOTenant** PowerShell.

Det er i øjeblikket ikke muligt at deaktivere kommentering på websteds-eller listeniveau. Vi håber, at du har disse kontrolelementer i en senere opdatering, sandsynligt i den første kvartal 2021.
