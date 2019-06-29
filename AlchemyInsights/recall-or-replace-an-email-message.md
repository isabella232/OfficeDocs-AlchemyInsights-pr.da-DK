---
title: Tilbagekalde eller erstatte en e-mail-meddelelse
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 170fbd632f0289a45d9497ac26fbe7f90cf88318
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356591"
---
# <a name="recall-or-replace-an-email-message"></a>Tilbagekalde eller erstatte en e-mail-meddelelse

- Du kan **kun tilbagekaldelse af meddelelser, der sendes til personer i organisationen**. Hvis meddelelsen blev sendt til en Gmail-adresse, for eksempel, ikke kan du huske den.
- Du kan **kun tilbagekaldelsesmeddelelsen, der sendes fra Outlook 2016 til PC**. Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på World Wide web, kan du trække den tilbage.
- Hvis du er administrator, kan du **tilbagekaldelsesmeddelelsen på vegne af brugere ved hjælp af PowerShell**. Du kan ikke trække meddelelser fra admin center. Rul ned til "Søg efter og slette e-mail-meddelelser i din organisation" for at få yderligere oplysninger.

***Tilbagekalde eller erstatte en e-mail-meddelelse, du har sendt***

1. Vælg mappen Sendt post i mapperuden i Outlook-vinduet til venstre.
2. Åbn den meddelelse, du vil tilbagekalde. Du skal dobbeltklikke for at åbne meddelelsen. At markere meddelelsen, så den vises i læseruden, kan du tilbagekalde meddelelsen ikke.
3. Vælg **Handlinger**under fanen meddelelse > **Tilbagekald denne meddelelse**.
4. Vælge **Slette ulæste kopier af denne meddelelse** eller **Slette ulæste kopier og erstatte med en ny meddelelse**og derefter klikke på **OK**.
5. Hvis du sender en meddelelse til udskiftning, Skriv meddelelsen, og vælg **Send**.
6. Lykkes eller ej af en tilbagekaldelse af meddelelse afhænger af modtagerens indstillinger i Outlook.

Yderligere herunder oplysninger, hvordan du kontrollere tilbagekaldelsen, [tilbagekaldelse eller erstatte en e-mail-meddelelse, du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Søge efter og slette e-mail-meddelelser i din organisation*** Hvis du vil søge efter og slette e-mail-meddelelser i din organisation, er det nemmest, hvis du er en global administrator. Hvis du ikke er en global administrator, skal kontoen føjes til rollegruppen eDiscovery Manager eller overholdelse søgning management rolle. Hvis du vil slette meddelelser, skal du deltage i rollegruppe organisationsstyring eller rollen søgning og Rens. Tilladelser til disse roller tildeles [sikkerhed & Overholdelsescenter](https://protection.office.com/).

1. [Opret et indhold søge](https://docs.microsoft.com/office365/securitycompliance/content-search) at finde meddelelsen slettes.
2. [Oprette forbindelse til sikkerhed & Overholdelsescenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Hvis du bruger MFA, se [Opret forbindelse til Office 365 sikkerhed & kompatibilitet Center PowerShell ved hjælp af godkendelse i flere niveauer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
