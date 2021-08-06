---
title: 902 (Synkroniseringsfejl på grund af dublerede objekter)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998781"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfejl på grund af dublerede objekter

Du modtager muligvis en af følgende fejlmeddelelser, når katalogsynkronisering afsluttes Microsoft 365:

- Kan ikke opdatere dette objekt i Microsoft Online Services, fordi følgende attributter, der er knyttet til dette objekt, har værdier, der måske allerede er knyttet til et andet objekt i din lokale mappe.

- Der findes allerede et synkroniseret objekt med den samme proxyadresse i Microsoft Online Services-kataloget.

- Dette objekt kan ikke opdateres, fordi de følgende attributter, der er knyttet til dette objekt, har værdier, der måske allerede er knyttet til et andet objekt i dine lokale adresselistetjenester: UserPrincipalName.

For at identificere og løse problemet skal du downloade og køre [IdFix DirSync-værktøjet til afhjælpning af fejl.](https://github.com/Microsoft/idfix)

Du kan finde flere oplysninger [i KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
