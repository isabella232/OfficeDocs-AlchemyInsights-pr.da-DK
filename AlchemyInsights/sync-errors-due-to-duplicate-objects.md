---
title: 902 (synkroniseringsfejl på grund af duplikerede objekter)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737335"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfejl på grund af dublerede objekter

Du får muligvis en af følgende fejlmeddelelser, når katalog synkroniseringen afsluttes i Microsoft 365:

- Det er ikke muligt at opdatere dette objekt i Microsoft Online Services, fordi de følgende attributter, der er knyttet til objektet, har værdier, der måske allerede er knyttet til et andet objekt i dit lokale katalog.

- Der findes allerede et synkroniseret objekt med den samme proxyadresse i din Microsoft Online Services-mappe.

- Kan ikke opdatere dette objekt, fordi følgende attributter, der er knyttet til objektet, har værdier, der muligvis allerede er knyttet til et andet objekt i dine lokale katalogtjenester: UserPrincipalName.

Hvis du vil identificere og løse problemet, skal du downloade og køre [værktøjet til afhjælpning af IdFix-fejl](https://www.microsoft.com/download/details.aspx?id=36832).

Du kan finde flere oplysninger i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
