---
title: Tilbagekald af Outlook på skrivebordet, eller Erstat en mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663984"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbagekalde eller erstatte en Outlook-mail

- Som administrator kan du **tilbagekalde meddelelser på vegne af brugere ved hjælp af PowerShell**. Du kan ikke tilbagekalde meddelelser fra administrations centeret.
- Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen**. Hvis meddelelsen blev sendt til en Gmail-adresse, kan du for eksempel ikke tilbagekalde den.
- Du kan **kun tilbagekalde meddelelser, der er sendt fra Outlook 2016 på pc'en**. Hvis en bruger sender en meddelelse ved hjælp af Outlook til Mac eller Outlook på internettet, kan du ikke tilbagekalde den.

Sådan tilbagekaldes eller erstattes en mail:

1. I mapperuden i venstre side af Outlook-vinduet skal du vælge mappen Sendt post.
1. Dobbeltklik på den meddelelse, du vil tilbagekalde, for at åbne den.
1. Vælg fanen **meddelelse** , og vælg derefter **handlinger**  >  **Tilbagekald denne meddelelse**.
1. Vælg **Slet ulæste kopier af denne meddelelse** , eller **Slet ulæste kopier, og Erstat med en ny meddelelse**, og vælg derefter **OK**.
1. Hvis du vil sende en erstatnings meddelelse, skal du skrive meddelelsen og derefter vælge **Send**.
1. Det lykkedes eller ikke lykkedes at tilbagekalde en meddelelse, afhænger af modtagerens indstillinger i Outlook. Du kan se, hvordan du kontrollerer tilbagekaldelsen, i [denne artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Søg efter og slet mails i din organisation

- Hvis du ikke er Global administrator, skal din konto føjes til rollen eDiscovery Manager-rolle eller overholdelses administrations rolle for at søge efter meddelelser. Hvis du vil slette meddelelser, skal du være medlem af gruppen organisations administrations rolle eller rollen søgning og sletning af administration. Tilladelser til disse roller tildeles i [sikkerheds-og overholdelses centeret](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Opret en indholdssøgning](https://docs.microsoft.com/microsoft-365/compliance/content-search) for at finde den besked, der skal slettes.
- [Opret forbindelse til sikkerheds-og overholdelses Center-PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Hvis du bruger multifaktorgodkendelse, skal du se [oprette forbindelse til Microsoft 365 Security and Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).