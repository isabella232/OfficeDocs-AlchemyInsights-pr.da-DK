---
title: Søge efter og slette mails i din organisation
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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523691"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Søge efter og slette mails i din organisation

Følg disse trin:

1. Hvis du ikke er global administrator, skal din konto føjes til **rollegruppen for eDiscovery Manager** eller administration af overholdelsessøgning for at søge efter **meddelelser.** Hvis du vil slette meddelelser, skal du deltage i **rollegruppen Organisationsadministration** eller **administrationsrollen Søg og tøm.** Tilladelser til disse roller tildeles i [Sikkerheds- & overholdelsescenter.](https://protection.office.com)
2. [Opret en indholdssøgning for](https://docs.microsoft.com/office365/securitycompliance/content-search) at finde den meddelelse, du vil slette.
3. [Opret forbindelse til Security & Compliance Center PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Hvis du bruger MFA, skal du se denne vejledning: Opret forbindelse til [Security & Compliance Center PowerShell ved hjælp af multifaktorgodkendelse](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Slet meddelelsen: Kør `New-ComplianceSearchAction` cmdlet'en for at slette meddelelsen. Slettede meddelelser flyttes til en brugers mappe genoprettelige elementer. Se trin 3 for at [få en eksempelkommando: Slet meddelelsen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
