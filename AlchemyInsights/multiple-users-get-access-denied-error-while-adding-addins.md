---
title: Flere brugere får fejlmeddelelsen Adgang nægtet, mens der tilføjes tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423480"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Flere brugere får fejlmeddelelsen Adgang nægtet, mens der tilføjes tilføjelsesprogrammer i Outlook

Du kan angive, hvilke administratorer i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til Outlook. Du kan også angive, hvilke brugere i organisationen der har tilladelse til at installere og administrere tilføjelsesprogrammer til eget brug.

Yderligere oplysninger kan finde [oplysninger under Angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Hvis du vil kontrollere, at du har tildelt tilladelser til en bruger, skal du erstatte med navnet på den <Role Name> rolle, der skal bekræftes, og køre følgende kommando i Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> -GetEffectiveUsers

I dette eksempel kan du se, hvordan du kan kontrollere, hvem du har tildelt tilladelser til at installere tilføjelsesprogrammer fra Office Store for organisationen.

Powershell

-Rolle "Org Marketplace Apps" -GetEffectiveUsers

I resultaterne skal Get-ManagementRoleAssignment gennemse posterne i kolonnen Effektive brugere.

Yderligere syntaks- og parameteroplysninger [finder du i Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 