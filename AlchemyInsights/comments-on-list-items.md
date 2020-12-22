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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724148"
---
# <a name="comments-on-list-items"></a>Kommentarer til listeelementer

Brugere kan se alle kommentarer på et listeelement og filtrere mellem visninger, der viser kommentarer eller aktiviteter relateret til et element.

Brugerne skal bemærke følgende, før de kan tilføje og slette kommentarer:

- Kommentarer følger de tilladelsesindstillinger, der er indbygget i SharePoint.
- Klassiske lister, der endnu ikke er bygget til at blive vist i moderne brugergrænseflader, f. eks. opgavelister, vil ikke have denne kommentarfunktion.
- Kommentering på lister i teams er ikke tilgængelig med denne version.
- Kommentarer indekseres ikke ved søgning.

Administratorer kan deaktivere denne funktion på organisationsniveau ved at ændre **CommentsOnListItemsDisabled** -parameteren i cmdlet'en **set-SPOTenant** PowerShell.

Det er i øjeblikket ikke muligt at deaktivere kommentering på websteds-eller listeniveau. Vi håber, at du har disse kontrolelementer i en senere opdatering, sandsynligt i den første kvartal 2021.
