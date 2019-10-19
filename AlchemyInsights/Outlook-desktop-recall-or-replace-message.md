---
title: Outlook-skrivebordet tilbagekaldelse eller Erstat en mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496105"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbagekalde eller erstatte en Outlook-mail

- Som administrator kan du **tilbagekalde meddelelser på vegne af brugere, som bruger PowerShell**. Du kan ikke tilbagekalde meddelelser fra administrationscenteret.
- Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**. Hvis beskeden blev sendt til en Gmail-adresse, kan du for eksempel ikke huske den.
- Du kan **kun tilbagekalde meddelelser, som er sendt fra Outlook 2016 på pc'en**. Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke huske den.

Sådan tilbagekaldes eller erstattes en mail:

1. Vælg mappen Sendt post i mapperuden til venstre i Outlook-vinduet.
1. Dobbeltklik på den meddelelse, du vil tilbagekalde, for at åbne den.
1. Vælg fanen **meddelelse** , og vælg derefter **handlinger** > **Tilbagekald denne meddelelse**.
1. Vælg **Slet ulæste kopier af denne meddelelse** , eller **Slet ulæste kopier, og Erstat med en ny meddelelse**, og vælg derefter **OK**.
1. Hvis du sender en erstatnings meddelelse, skal du skrive meddelelsen og derefter vælge **Send**.
1. Succesen eller fiaskoen for en meddelelse tilbagekaldelse afhænger af modtagerens indstillinger i Outlook. Se [denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)for at få trin til at kontrollere tilbagekaldelsen.

Søg efter og slet e-mail-meddelelser i din organisation

- Hvis du ikke er Global administrator, skal din konto føjes til rollen eDiscovery Manager eller styring af Overholdelsessøgning for at søge efter meddelelser. Hvis du vil slette meddelelser, skal du tilmelde dig organisations administrations rollegruppen eller rollen Søg og fjernadministration. Tilladelserne til disse roller tildeles i [Security and Compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opret en indholdssøgning](https://docs.microsoft.com/office365/securitycompliance/content-search) for at finde den meddelelse, der skal slettes.
- [Opret forbindelse til Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruger multifaktorgodkendelse, kan du se under [Opret forbindelse til Office 365 Security and Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).