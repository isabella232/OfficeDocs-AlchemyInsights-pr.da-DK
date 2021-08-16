---
title: Flere brugere kan ikke se tilføjelses in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011798"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Flere brugere kan ikke se tilføjelses in Outlook

Hvis du tester Outlook, og ingen vises som det første fejlfindingstrin, skal du bruge **Get-OrganizationConfig** PowerShell-cmdlet'en til at forespørge på _appsForOfficeEnabled-parameteren._ Hvis forespørgslen returnerer værdien **Falsk,** skal du  indstille denne parameter til Sand ved hjælp af cmdlet'en **Set-OrganizationConfig,** så tilføjelses ins vises som forventet.

Vi anbefaler ikke, at _parameteren AppsForOfficeEnabled_ er angivet til **Falsk**. En værdi af **Falsk** tilsidesætter alle ovenstående administrative indstillinger og brugerrolleindstillinger og forhindrer nye apps i at blive aktiveret af alle brugere i organisationen.

Du kan finde flere oplysninger [under Angive de administratorer og brugere, der kan installere](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)og administrere tilføjelsesprogrammet for Outlook .