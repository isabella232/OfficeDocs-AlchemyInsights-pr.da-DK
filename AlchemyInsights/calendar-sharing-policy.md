---
title: 618 Politik for kalenderdeling
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372993"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Politikfejl ved deling af en kalender

1. Bedød en af følgende fremgangsmåder, alt efter hvad der passer til din situation:
    - Opret forbindelse til Exchange Online ved hjælp af Remote PowerShell. Yderligere oplysninger finder du i [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Åbn Exchange Management Shell på den lokale server.
2. Find ud af, hvilken delingspolitik brugeren har fået tildelt. Det kan du gøre ved at køre følgende kommando og notere den returnerede politik:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Opdater delingspolitikken for brugeren. Dette gøres ved at benytte følgende fremgangsmåde:
    - Åbn Exchange Administration.
    - Klik på **Organisation**, og dobbeltklik derefter på den politik, der er tildelt brugeren under **Individuel deling**. Det er den politik, der blev returneret i trin 2.
    - Vælg det kalenderdelingsniveau, du vil tillade, under **Angiv, hvilke oplysninger du vil dele**, på siden Delingsregel. Klik på **Gem**.

Du kan finde flere oplysninger under: ["Politik tillader ikke tildeling af tilladelser på dette niveau til en eller flere af modtagernes)"-fejl, når brugeren forsøger at dele kalenderen](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
