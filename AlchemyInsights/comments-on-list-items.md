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
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995472"
---
# <a name="comments-on-list-items"></a>Kommentarer til listeelementer

Brugere kan få vist alle kommentarer på et listeelement og filtrere mellem visninger, der viser kommentarer eller aktivitet relateret til et element.

Brugerne skal være opmærksom på følgende, før de kan tilføje og slette kommentarer:

- Kommentarer følger de tilladelsesindstillinger, der er forbundet med SharePoint.
- Klassiske lister, der endnu ikke er oprettet til at blive vist i moderne brugergrænseflader, f.eks. opgavelister, vil ikke have denne kommentarfunktion.
- Kommentering på lister i Teams er ikke tilgængelig med denne version.
- Kommentarer indekseres ikke af Søg.

Administratorer kan deaktivere denne funktion på organisationsniveau ved at ændre **CommentsOnListItemsDisabled-parameteren** i **Set-SPOTenant** PowerShell-cmdlet'en.

Det er i øjeblikket ikke muligt at deaktivere kommentar på websteds- eller listeniveau. Vi håber at have disse kontrolfunktioner i en senere opdatering, sandsynligvis i første kvartal 2021.
