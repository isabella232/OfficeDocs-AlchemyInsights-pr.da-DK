---
title: 618 kalender delings politik
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684224"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Politik fejl ved deling af en kalender

1. Gør et af følgende, afhængigt af din situation:
    - Opret forbindelse til Exchange Online ved hjælp af Remote PowerShell. Hvis du vil have mere at vide, skal du se [oprette forbindelse til Exchange Online ved hjælp af Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Åbn Exchange Management Shell på den lokale server.
2. Find ud af, hvilken delings politik der er tildelt brugeren. Hvis du vil gøre dette, skal du køre følgende kommando og bemærke, at den returnerede politik:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Opdater delings politikken for brugeren. Dette gøres ved at benytte følgende fremgangsmåde:
    - Åbn Exchange administration.
    - Klik på **organisation**, og dobbeltklik derefter på den politik, der er tildelt brugeren under **individuel deling**. Dette er den politik, der blev returneret i trin 2.
    - På siden delings regel skal du vælge det niveau for kalender deling, du vil tillade under **angive, hvilke oplysninger du vil dele**. Klik på **Gem**.

Du kan finde flere oplysninger under: ["politikken tillader ikke, at der tildeles tilladelser på dette niveau til en eller flere af modtager meddelelsen", når brugeren forsøger at dele kalender](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
