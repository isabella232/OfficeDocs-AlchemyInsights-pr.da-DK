---
title: Tilbagekald eller erstat en mail
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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024380"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Tilbagekald eller erstat en mail i Microsoft 365

- Du kan **kun tilbagekalde meddelelser, der sendes til personer i organisationen.** Hvis meddelelsen f.eks. blev sendt til en Gmail-adresse, kan du ikke tilbagekalde den.
- Du kan **kun tilbagekalde meddelelser, der er sendt Outlook til pc.** Hvis en bruger sender en meddelelse ved Outlook til Mac eller Outlook på internettet, kan du ikke tilbagekalde den.
- Som lejeradministrator kan du tilbagekalde meddelelser på vegne af brugere ved hjælp af **PowerShell** (Få mere at vide under: Søg efter [og slet mails](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Du kan ikke tilbagekalde meddelelser fra Administration. Rul ned til "Søg efter og slet mails i din organisation" for at få flere oplysninger.

**Tilbagekald eller erstat en mail, du har sendt**

1. I mapperuden til venstre for vinduet Outlook du vælge mappen Sendt post.
2. Åbn den meddelelse, du vil tilbagekalde. Du skal dobbeltklikke for at åbne meddelelsen. Hvis du vælger meddelelsen, så den vises i læseruden, kan du ikke tilbagekalde meddelelsen.
3. På fanen Meddelelse skal du vælge Handlinger  >  **Tilbagekald denne meddelelse**.
4. Vælg **Slet ulæste kopier af denne meddelelse** eller Slet **ulæste kopier af denne meddelelse, og erstat dem med en ny meddelelse,** og vælg derefter **OK**.
5. Hvis du sender en erstatningsmeddelelse, skal du skrive meddelelsen og derefter vælge **Send**.
6. Om en tilbagekaldelse lykkes eller mislykkes afhænger af modtagerens indstillinger i Outlook.

Du kan finde flere oplysninger, herunder hvordan du kontrollerer tilbagekaldelsen, under [Tilbagekald eller erstat en mail, du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Hvis du vil søge efter og slette mails i din organisation***, er det nemmest, hvis du er global administrator. Hvis du ikke er global administrator, skal din konto føjes til rollegruppen eDiscovery Manager eller til rollen som styring af overholdelsessøgning. Hvis du vil slette meddelelser, skal du tilmelde dig rollegruppen Organisationsadministration eller administration af søgning og tømning. Tilladelser til disse roller tildeles i [Sikkerheds- & overholdelsescenter](https://protection.office.com/).

1. [Opret en indholdssøgning for](https://docs.microsoft.com/microsoft-365/compliance/content-search) at finde den meddelelse, du vil slette.
2. [Forbind til Security & Compliance Center PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Hvis du bruger MFA (multifaktorgodkendelse), skal du se Forbind Microsoft 365 Security & Compliance Center PowerShell ved hjælp af [multifaktorgodkendelse.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
