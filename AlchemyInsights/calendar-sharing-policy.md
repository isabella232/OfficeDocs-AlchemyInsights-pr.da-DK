---
title: Politik for deling af kalender 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091593"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Politikfejl ved deling af en kalender

1. Gør et af følgende, som er relevant for din situation:
    - Forbind at Exchange Online ved hjælp af Remote PowerShell. Du kan finde flere oplysninger [i Forbind at Exchange Online ved hjælp af Remote PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - På den lokale server skal du åbne Exchange Management Shell.
2. Bestem den delingspolitik, der er tildelt brugeren. For at gøre dette skal du køre følgende kommando og notere den returnerede politik:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Opdater brugerens delingspolitik. Dette gøres ved at benytte følgende fremgangsmåde:
    - Åbn Exchange Administration.
    - Klik **på** Organisation , og dobbeltklik derefter på den politik, der er tildelt brugeren, under **Individuel deling**. Dette er den politik, der blev returneret i trin 2.
    - På siden Delingsregel skal du vælge det kalenderdelingsniveau, du vil tillade, under **Angiv, hvilke oplysninger du vil dele**. skal du **klikke på Gem.**

Du kan finde flere oplysninger under: "Politikken tillader ikke, at der tildeles tilladelser på dette niveau til en eller flere af [modtagerens/modtagernes"-fejl,](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)når brugeren forsøger at dele kalender.
