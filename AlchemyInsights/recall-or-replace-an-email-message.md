---
title: Tilbagekalde eller erstatte en mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509450"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Tilbagekalde eller erstatte en mail i Microsoft 365

- Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**. Hvis meddelelsen f.eks.
- Du kan **kun tilbagekalde meddelelser, der er sendt fra Outlook 2016 til pc'en**. Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke huske den.
- Hvis du er administrator, kan du **tilbagekalde meddelelser på vegne af brugere ved hjælp af PowerShell**. Du kan ikke tilbagekalde meddelelser fra Administration. Rul ned til "Søg efter og slet mails i organisationen" for at få flere oplysninger.

**Tilbagekalde eller erstatte en mail, du har sendt**

1. Vælg mappen Sendt post i mapperuden til venstre i Outlook-vinduet.
2. Åbn den meddelelse, du vil tilbagekalde. Du skal dobbeltklikke for at åbne meddelelsen. Hvis du vælger meddelelsen, så den vises i læseruden, kan du ikke tilbagekalde meddelelsen.
3. Vælg **Handlinger**  >  **Tilbagekald denne meddelelse**under fanen Meddelelse .
4. Vælg **Slet ulæste kopier af denne meddelelse** eller Slet **ulæste kopier, og erstat med en ny meddelelse**, og vælg derefter **OK**.
5. Hvis du sender en erstatningsmeddelelse, skal du skrive meddelelsen og derefter vælge **Send**.
6. Hvis en meddelelse igen igen lykkes eller mislykkes, afhænger af modtagernes indstillinger i Outlook.

Du kan finde flere oplysninger, herunder hvordan du kontrollerer tilbagekaldelsen, under [Tilbagekalde eller erstatte en mail, du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Søge efter og slette mails i din organisation*** Hvis du vil søge efter og slette mails i din organisation, er det nemmest, hvis du er global administrator. Hvis du ikke er global administrator, skal din konto føjes til rollegruppen eDiscovery Manager eller til rollen Administration af overholdelsessøgning. Hvis du vil slette meddelelser, skal du deltage i rollegruppen Organisationsstyring eller rollen Søg og fjern administration. Tilladelser til disse roller tildeles i [Sikkerhedscenter & overholdelsescenter](https://protection.office.com/).

1. [Opret en indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/content-search) for at finde den meddelelse, der skal slettes.
2. [Opret forbindelse til Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Hvis du bruger MFA, skal du se [Oprette forbindelse til Microsoft 365-sikkerhed & Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
