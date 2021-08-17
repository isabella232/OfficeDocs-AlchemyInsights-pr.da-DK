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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892041"
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
