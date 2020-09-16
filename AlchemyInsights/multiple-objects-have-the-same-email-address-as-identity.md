---
title: Flere objekter har den samme mailadresse som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724609"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Flere objekter har den samme mailadresse som identitet

**Flere objekter**

En af de almindelige årsager til denne fejl er ikke muligt at omdirigere en Outlook Web Access-anmodning korrekt i en tilstedeværelse af flere objekter, der har den samme mailadresse som identitet. Hvis du vil finde disse objekter, skal du køre følgende kommandoer:

· Hent-modtager <email address>

· Hent-bruger <email address>

· Get-User <email address> -SoftDeletedUser

· Hent-kontakt <email address>

· Get-postkassen <email address> -PublicFolder

· Get-postkassen <email address> -IncludeSoftDeletedMailbox

· Get-postkassen <email address> -InactiveMailboxOnly

Du kan løse problemet ved at fjerne flere objekter med samme mail-id og sørge for, at der er et enkelt objekt med det specifikke mail-id, og at modtager typen er UserMailbox.

**Den samme adresse bruges til forretnings-og forbruger postkasser**

En anden årsag er, når den samme adresse bruges til forretnings-og forbruger postkasser. I dette tilfælde skal brugeren ændre vedkommendes primære forbruger alias, indtil Café understøtter dette scenarie. Dette er en permanent fejl, der ikke forsvinder uden indgriben.

Hvis du vil have mere at vide, skal du se [ændre mailadressen eller telefonnummeret til din Microsoft-konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).