---
title: Outlook Tilbagekalde eller erstatte en mail på skrivebordet
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918389"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Tilbagekald eller erstat Outlook mail

- Som administrator kan du tilbagekalde meddelelser **på vegne af brugere ved hjælp af PowerShell.** Du kan ikke tilbagekalde meddelelser fra Administration.
- Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen.** Hvis meddelelsen f.eks. blev sendt til en Gmail-adresse, kan du ikke tilbagekalde den.
- Du kan **kun tilbagekalde meddelelser, der er Outlook 2016 på pc'en.** Hvis en bruger sender en meddelelse ved Outlook til Mac eller Outlook på internettet, kan du ikke tilbagekalde den.

Sådan tilbagekaldes eller erstattes en mail:

1. I mapperuden til venstre for vinduet Outlook du vælge mappen Sendt post.
1. Dobbeltklik på den meddelelse, du vil tilbagekalde, for at åbne den.
1. Vælg fanen **Meddelelse,** og vælg derefter **Tilbagekald**  >  **denne meddelelse.**
1. Vælg **Slet ulæste kopier af denne meddelelse** eller Slet **ulæste kopier af denne meddelelse, og erstat dem med** en ny meddelelse, og vælg derefter **OK**.
1. Hvis du sender en erstatningsmeddelelse, skal du skrive meddelelsen og derefter vælge **Send**.
1. Om en tilbagekaldelse lykkes eller mislykkes afhænger af modtagerens indstillinger i Outlook. Du kan finde trin til at kontrollere tilbagekaldelsen i [denne artikel.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Søg efter og slet mails i din organisation

- Hvis du ikke er global administrator, skal din konto føjes til eDiscovery Manager-rollen eller administrationsrollen til overholdelsessøgning for at søge efter meddelelser. Hvis du vil slette meddelelser, skal du tilmelde dig rollegruppen Organisationsadministration eller administration af søgning og tømning. Tilladelser for disse roller tildeles i [Sikkerheds- og overholdelsescenter.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Opret en indholdssøgning for](https://docs.microsoft.com/microsoft-365/compliance/content-search) at finde den meddelelse, du vil slette.
- [Forbind til Security and Compliance Center PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Hvis du bruger multifaktorgodkendelse, skal du se Forbind Microsoft 365 security and Compliance Center PowerShell ved hjælp [af multifaktorgodkendelse.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)