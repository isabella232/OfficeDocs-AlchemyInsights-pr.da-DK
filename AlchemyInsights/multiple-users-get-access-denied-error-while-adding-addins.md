---
title: Flere brugere får fejlen Adgang nægtet, når de tilføjer tilføjelser i Outlook
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
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065386"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Flere brugere får fejlen Adgang nægtet, når de tilføjer tilføjelser i Outlook

Du kan angive, hvilke administratorer i organisationen der har tilladelse til at installere og administrere tilføjelser til Outlook. Du kan også angive, hvilke brugere i organisationen der har tilladelse til at installere og administrere tilføjelser til eget brug.

Du kan få mere [at vide under Angive de administratorer og brugere,](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)der kan installere og administrere tilføjelsesprogrammet for Outlook .

For at bekræfte, at du har tildelt tilladelser for en bruger, skal du erstatte med navnet på den rolle, der skal bekræftes, og køre følgende kommando <Role Name> i Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers

I dette eksempel kan du se, hvordan du kan bekræfte, hvem du har tildelt tilladelser til at installere tilføjelser fra Office Store for organisationen.

PowerShell

-Rolle "Org Marketplace-apps" -GetEffectiveUsers

I resultaterne, Get-ManagementRoleAssignment, skal du gennemse posterne i kolonnen Effektive brugere.

Du kan finde detaljerede oplysninger om syntaks og [parameter i Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 