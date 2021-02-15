---
title: Blokere brugerbaserede mailsignaturer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243318"
---
# <a name="block-user-made-email-signatures"></a>Blokere brugerbaserede mailsignaturer

Følgende løsning gælder kun for mailsignaturer, der er oprettet i Outlook på internettet. Du kan kun blokere signaturer i Outlook-appen, hvis du har en lokal Exchange Server.

1. Vælg Administration Exchange **i**  >  **Administration.**
2. Klik **på tilladelser i** Outlook Web  >  **App-politikker.**
3. Vælg politikken, og klik derefter på blyantsikonet for at redigere den.
4. Klik **på funktioner** Flere  >  **indstillinger.**
5. Fjern **markeringen i afkrydsningsfeltet** **Mailsignatur under** Brugeroplevelse, og klik derefter på **Gem.**

**Vigtigt!** Hvis der blev tilføjet en signatur, før dette afkrydsningsfelt blev fjernet, vil brugeren stadig kunne bruge den. Bed dem om at fjerne den.
