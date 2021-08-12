---
title: Søg efter og slet mails i din organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948877"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Søg efter og slet mails i din organisation

Følg disse trin:

1. Hvis du ikke er global administrator, skal din konto føjes til **rollegruppen eDiscovery Manager** eller administration af overholdelsessøgning for at søge efter **meddelelser.** Hvis du vil slette meddelelser, skal du tilmelde dig **rollegruppen Organisationsadministration** eller **administrationsrollen Søg og tøm.** Tilladelser til disse roller tildeles i [Sikkerheds- & overholdelsescenter.](https://protection.office.com)
2. [Opret en indholdssøgning for](https://docs.microsoft.com/office365/securitycompliance/content-search) at finde den meddelelse, du vil slette.
3. [Forbind til Security & Compliance Center PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Hvis du bruger MFA, skal du se denne vejledning: Forbind til Security & Compliance Center PowerShell ved hjælp af [multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Slet meddelelsen: Kør `New-ComplianceSearchAction` cmdlet'en for at slette meddelelsen. Slettede meddelelser flyttes til en brugers mappe genoprettelige elementer. Se en eksempelkommando i [Trin 3: Slet meddelelsen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
