---
title: Flere brugere kan ikke se tilføjelsesprogrammer i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197839"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Flere brugere kan ikke se tilføjelsesprogrammer i Outlook

Hvis du tester Outlook-tilføjelsesprogrammer, og ingen vises, skal du som et første fejlfindingstrin bruge Cmdlet'en **Get-OrganizationConfig** PowerShell til at forespørge på parameteren _AppsForOfficeEnabled._ Hvis forespørgslen returnerer en værdi af **Falsk**, skal du angive denne parameter til **Sand** ved hjælp af **set-OrganizationConfig-cmdlet'en,** så tilføjelsesprogrammer vises som forventet.

Vi anbefaler ikke, at parameteren _AppsForOfficeEnabled_ er angivet til **False**. En værdi af **Falsk** tilsidesætter alle ovenstående indstillinger for administrative og brugeriske rolle og forhindrer, at nye apps aktiveres af en bruger i organisationen.

Du kan finde flere oplysninger [under Angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).