---
title: Outlook-computer tilbagekalder eller erstatter en mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502313"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbagekalde eller erstatte en Outlook-mail

- Som administrator kan du **tilbagekalde meddelelser på vegne af brugere, der bruger PowerShell**. Du kan ikke tilbagekalde meddelelser fra Administration.
- Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**. Hvis meddelelsen f.eks.
- Du kan **kun tilbagekalde meddelelser, der er sendt fra Outlook 2016 på pc'en**. Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke huske den.

Sådan tilbagekalder eller erstatter du en mail:

1. Vælg mappen Sendt post i mapperuden til venstre i Outlook-vinduet.
1. Dobbeltklik på den meddelelse, du vil huske for at åbne den.
1. Vælg fanen **Meddelelse,** og vælg derefter **Handlinger**  >  **Tilbagekald denne meddelelse**.
1. Vælg **Slet ulæste kopier af denne meddelelse** eller Slet **ulæste kopier, og erstat med en ny meddelelse**, og vælg derefter **OK**.
1. Hvis du sender en erstatningsmeddelelse, skal du skrive meddelelsen og derefter vælge **Send**.
1. Hvis en meddelelse igen igen lykkes eller mislykkes, afhænger af modtagerens indstillinger i Outlook. Du kan se, hvordan du kommer til at kontrollere tilbagekaldelsen, i [denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søge efter og slette mails i din organisation

- Hvis du ikke er global administrator, skal din konto føjes til rollen eDiscovery Manager eller administrationsrollen Overholdelsessøgning for at søge efter meddelelser. Hvis du vil slette meddelelser, skal du deltage i rollegruppen Organisationsstyring eller rollen Søg og fjern administration. Tilladelser til disse roller tildeles i [Sikkerheds- og overholdelsescenteret](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opret en indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/content-search) for at finde den meddelelse, der skal slettes.
- [Opret forbindelse til PowerShell til Sikkerheds- og Overholdelsescenter](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruger multifaktorgodkendelse, skal du se [Oprette forbindelse til Microsoft 365-sikkerheds- og Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).