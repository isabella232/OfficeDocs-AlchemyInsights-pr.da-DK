---
title: Enkeltbrugere kan ikke se tilføjelses in Outlook
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
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050652"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Enkeltbrugere kan ikke se tilføjelses in Outlook

Brugeren kan være en del af en rolle, der ikke har den korrekte AppsForOfficeEnabled-parameter. Kør denne cmdlet for at finde ud af, om den korrekte rolle er knyttet til brugeren:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com –Delegerings$$false | Format-Table -Autorolle,RolleAssigneeNavn,RolleAssigneeType

Du kan få mere at [vide under Angiv de administratorer og brugere,](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)der kan installere og administrere tilføjelsesprogrammet for Outlook .
