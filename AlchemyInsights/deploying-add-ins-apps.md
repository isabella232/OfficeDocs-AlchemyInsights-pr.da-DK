---
title: Installation af tilføjelsesprogrammet til Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/30/2021
ms.locfileid: "52124965"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Installation af tilføjelsesprogrammet til Microsoft 365 Apps

Centraliseret udrulning er den anbefalede metode til Office udrulning af tilføjelsesprogrammet til brugere og grupper i organisationen. Hvis du vil installere tilføjelsesprogrammet, skal du følge nedenstående trin:

**Bemærk!** Hvis du vil installere tilføjelsesprogrammer til Office som individuel bruger, skal du se Få vist, administrer og installér tilføjelsesprogrammer [i Office programmer.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Sørg også for, at individuel anskaffelse af Office Store er aktiveret. 

1. Sørg for, at dit miljø opfylder kravene til udrulning af tilføjelser ved hjælp af Centraliseret udrulning. Du kan få mere at vide under [Krav](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Gå til **Indstillinger**  >  **integrerede apps** Hent  >  **apps** i Microsoft 365 Administration for at installere tilføjelsesprogrammer. 

Bemærkninger: 

- Integrerede apps kræver, at administratoren har globale administrator- Exchange administratortilladelser.

- Når du installerer tilføjelser til flere brugere, anbefaler vi, at du foretager tildelinger ved hjælp af grupper i stedet for individuelle brugere. Du kan få mere at [vide under Overvejelser ved tildeling af et tilføjelsesprogrammet til brugere og grupper.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centraliseret udrulning understøtter ikke brugere i indlejrede grupper eller grupper, der har overordnede grupper. Du kan få mere at [vide under Bruger- og gruppetildelinger.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Sørg for, at Microsoft 365 GUID (App Management Service: '0517ffae-825d-4aff-999e-3f2336b8a20a') er aktiveret til at logge på. Du kan få mere at vide [under Konfigurere appegenskaber](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Hvis du oplever problemer med installation af tilføjelsesprogrammer ved hjælp af integrerede apps, kan du prøve at [installere ved hjælp af tilføjelsesprogrammer](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Du kan finde flere oplysninger under:

[Installér tilføjelser i Administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Administrer tilføjelser i Administration](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Brug de Centraliserede udrulning af PowerShell-cmdlet'er til at administrere tilføjelsesinstallationer](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicere Office-tilføjelsesprogrammet ved hjælp af Centraliseret udrulning via Microsoft 365 Administration](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Fejlfinding: Brugeren kan ikke se tilføjelsesprogram](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Fejlfinding af brugerfejl Office tilføjelsesprogram](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)