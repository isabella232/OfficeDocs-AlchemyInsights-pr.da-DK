---
title: Flere objekter har samme mailadresse som identitet
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
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011906"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Flere objekter har samme mailadresse som identitet

**Flere objekter**

En af de almindelige årsager til denne fejl er, at du ikke kan distribuere en Outlook Web Access-anmodning korrekt, hvis der er flere objekter med samme mailadresse som identitet. Kør følgende kommandoer for at finde disse objekter:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Du kan løse problemet ved at fjerne flere objekter med den samme mailidentitet og sørge for, at der er et enkelt objekt med den specifikke mailidentitet, og at modtagertypen er UserMailbox.

**Samme adresse bruges til virksomheds- og forbrugerpostkasser**

En anden årsag er, når den samme adresse bruges til postkasser til virksomheder og forbrugere. I dette tilfælde skal brugeren ændre brugerens primære forbrugeralias, indtil Cafe understøtter dette scenarie. Dette er en permanent fejl, der ikke forsvinder uden handling.

Hvis du vil have mere [at vide, skal du se Ændre mailadressen eller telefonnummeret til din Microsoft-konto.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)