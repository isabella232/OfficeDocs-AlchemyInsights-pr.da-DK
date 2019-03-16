---
title: Outlook stationære tilbagekaldelse eller erstatte en e-mail-meddelelse
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657038"
---
# <a name="recall-or-replace-an-email-message"></a>Tilbagekalde eller erstatte en e-mail-meddelelse

- Som administrator kan du **tilbagekaldelse af meddelelser på vegne af brugere ved hjælp af PowerShell**. Du kan ikke trække meddelelser fra admin center.
- Du kan **kun tilbagekaldelse af meddelelser, der sendes til personer i organisationen**. Hvis meddelelsen blev sendt til en Gmail-adresse, for eksempel, ikke kan du huske den.
- Du kan **kun tilbagekaldelsesmeddelelsen, der sendes fra Outlook 2016 på PC'EN**. Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på World Wide web, kan du trække den tilbage.

Du tilbagekalder eller erstatter en e-mail-meddelelse:

1. Vælg mappen Sendt post i mapperuden i Outlook-vinduet til venstre.
1. Dobbeltklik på den meddelelse, du vil tilbagekalde for at åbne den.
1. Vælg fanen **meddelelse** og derefter vælge **Handlinger** > **Tilbagekald denne meddelelse**.
1. Vælg **Slette ulæste kopier af denne meddelelse** eller **Slette ulæste kopier og erstatte med en ny meddelelse**, og klik derefter på **OK**.
1. Hvis du sender en meddelelse til udskiftning, Skriv meddelelsen, og vælg derefter **Send**.
1. Lykkes eller ej af en tilbagekaldelse af meddelelse afhænger af modtagerens indstillinger i Outlook. Hvordan at kontrollere tilbagekaldelsen, finder du [i denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søge efter og slette e-mail-meddelelser i din organisation

- Hvis du ikke er en global administrator, skal kontoen føjes til eDiscovery lederrolle eller rollen overholdelse søgning til at søge efter meddelelser. Hvis du vil slette meddelelser, skal du deltage i rollegruppe organisationsstyring eller rollen søgning og Rens. Der tildeles tilladelser til disse roller i [center for sikkerhed og kompatibilitet](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opret et indhold søge](https://docs.microsoft.com/office365/securitycompliance/content-search) at finde meddelelsen slettes.
- [Oprette forbindelse til sikkerhed og PowerShell Overholdelsescenter](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruger godkendelse i flere niveauer, kan du se [Opret forbindelse til Office 365 sikkerhed og kompatibilitet Center PowerShell ved hjælp af godkendelse i flere niveauer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).