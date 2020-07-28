---
title: Flere objekter har samme mailadresse som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438933"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Flere objekter har samme mailadresse som identitet

**Flere objekter**

En af de almindelige årsager til denne fejl er ikke at kunne distribuere en Outlook Web Access-anmodning korrekt i nærheden af flere objekter med samme mailadresse som identitet. Hvis du vil finde disse objekter, skal du køre følgende kommandoer:

· Hent modtager<email address>

· Hent bruger<email address>

· Get-User <email address> -SoftDeletedUser

· Get-Kontakt<email address>

· Hent postkasse <email address> -Offentligfolder

· Hent postkasse <email address> -IncludeSoftDeletedMailbox

· Hent postkasse <email address> -InaktivMailboxKun

Du kan løse problemet ved at fjerne flere objekter med den samme mailidentitet og sørge for, at der er et enkelt objekt med den specifikke e-mail-identitet, og at modtagertypen er UserMailbox.

**Samme adresse bruges til virksomheds- og forbrugerpostkasser**

En anden årsag er, når den samme adresse bruges til virksomheds- og forbrugerpostkasser. I dette tilfælde skal brugeren ændre sit primære forbrugeralias, indtil Cafe understøtter dette scenarie. Dette er en permanent fejl, der ikke går væk uden indgriben.

Du kan finde flere oplysninger [under Ændre mailadressen eller telefonnummeret til din Microsoft-konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).