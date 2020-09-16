---
title: Flere brugere får adgang nægtet-fejl under tilføjelse af tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724357"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Flere brugere får adgang nægtet-fejl under tilføjelse af tilføjelsesprogrammer i Outlook

Du kan angive, hvilke administratorer i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til Outlook. Du kan også angive, hvilke brugere i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til deres eget brug.

Hvis du vil have mere at vide, skal du se [angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Hvis du vil bekræfte, at du har fået tildelt tilladelser for en bruger, skal du erstatte <Role Name> med navnet på rollen for at bekræfte og køre følgende kommando i Exchange Online PowerShell:

Get-ManagementRoleAssignment-Role " <Role Name> "-GetEffectiveUsers

I dette eksempel kan du se, hvordan du kan se, hvem du har tildelt tilladelser til at installere tilføjelsesprogrammer fra Office store for organisationen.

PowerShell

-Role "org Marketplace-apps"-GetEffectiveUsers

I resultaterne, Get-ManagementRoleAssignment, skal du gennemgå posterne i kolonnen effektive brugere.

Du kan finde detaljerede oplysninger om syntaks og parameter under [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 