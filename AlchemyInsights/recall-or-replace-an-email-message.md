---
title: Tilbagekalde eller erstatte en e-mail-meddelelse
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799198"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Tilbagekalde eller erstatte en e-mail-meddelelse i Microsoft 365

- Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**. Hvis meddelelsen blev sendt til en Gmail-adresse, kan du for eksempel ikke tilbagekalde den.
- Du kan **kun tilbagekalde meddelelser, der er sendt fra Outlook 2016 til PC**. Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke tilbagekalde den.
- Hvis du er administrator, kan du **tilbagekalde meddelelser på vegne af brugere ved hjælp af PowerShell**. Du kan ikke tilbagekalde meddelelser fra administrations centeret. Rul ned til "Søg efter og slet mails i organisationen" for at få flere oplysninger.

**Tilbagekalde eller erstatte en mail, som du har sendt**

1. I mapperuden i venstre side af Outlook-vinduet skal du vælge mappen Sendt post.
2. Åbn den meddelelse, du vil tilbagekalde. Du skal dobbeltklikke for at åbne meddelelsen. Hvis du vælger meddelelsen, så den vises i læseruden, kan du ikke tilbagekalde meddelelsen.
3. På fanen meddelelse skal du vælge **handlinger**  >  **Tilbagekald denne meddelelse**.
4. Vælg **Slet ulæste kopier af denne meddelelse** , eller **Slet ulæste kopier, og Erstat med en ny meddelelse**, og vælg derefter **OK**.
5. Hvis du vil sende en erstatnings meddelelse, skal du skrive meddelelsen og derefter vælge **Send**.
6. Hvis en meddelelses tilbagekaldelse lykkes eller ej, afhænger af modtagernes indstillinger i Outlook.

Du kan finde flere oplysninger, herunder hvordan du kontrollerer tilbagekaldelsen, under [tilbagekald eller Erstat en mail, du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Søg efter og slet mails i din organisation*** Hvis du vil søge efter og slette mails i organisationen, er det nemmest, hvis du er Global administrator. Hvis du ikke er en global administrator, skal din konto føjes til rollegruppen eDiscovery Manager eller for rollen overholdelses Search Management. Hvis du vil slette meddelelser, skal du være medlem af gruppen organisations administrations rolle eller rollen søgning og sletning af administration. Tilladelser til disse roller tildeles i [sikkerheds & Overholdelsescenter](https://protection.office.com/).

1. [Opret en indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/content-search) for at finde den besked, der skal slettes.
2. [Opret forbindelse til sikkerheds & Compliance Center-PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Hvis du bruger MFA, skal du se [oprette forbindelse til Microsoft 365 security & Compliance Center PowerShell med multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
