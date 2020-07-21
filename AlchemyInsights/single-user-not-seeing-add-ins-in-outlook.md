---
title: En enkelt bruger kan ikke se tilføjelsesprogrammer i Outlook
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
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197831"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>En enkelt bruger kan ikke se tilføjelsesprogrammer i Outlook

Brugeren kan være en del af en rolle, der ikke har den korrekte Parameter AppsForOfficeEnabled. Kør denne cmdlet for at finde ud af, om den korrekte rolle er knyttet til brugeren:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Uddelegering $false | Format-tabel -auto-rolle,RolleassigneeNavn,RolleassigneeType

Du kan finde flere oplysninger under [Angive de administratorer og brugere, der kan installere og administrere tilføjelsesprogrammer til Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
