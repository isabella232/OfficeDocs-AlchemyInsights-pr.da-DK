---
title: Manglende mails i karantæne
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329656"
---
# <a name="missing-emails-in-quarantine"></a>Manglende mails i karantæne

Administratorer kan [få vist, slippe eller slette disse meddelelser](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

I portalen Microsoft 365 Defender på <https://security.microsoft.com> skal du gå til **Gennemse** \> **karantæne**. Eller du kan bruge til at gå direkte **til siden** <https://security.microsoft.com/quarantine> Karantæne.  

Du kan finde flere oplysninger om de søge-/filterværdier, du kan bruge, under Administrer meddelelser og filer, der er sat i karantæne [som administrator i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

De cmdlet'er, du bruger til at få vist og administrere meddelelser og filer i karantæne, er:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [ForhåndsvisningskarantæneMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Bemærk, at denne cmdlet kun er til meddelelser, ikke filer fra Pengeskab Vedhæftede filer til SharePoint, OneDrive eller Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
