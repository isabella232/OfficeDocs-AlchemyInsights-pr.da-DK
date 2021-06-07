---
title: Administrere registrering af webinarer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793706"
---
# <a name="manage-webinar-registration"></a>Administrere registrering af webinarer

Du styrer, hvem der kan tilmelde dig Teams webinarer ved hjælp Teams Powershell-kommandoer. Hvis du vil Teams Powershell, skal [du se Teams PowerShell.](/microsoftteams/teams-powershell-install) 

*WhoCanRegister er som standard* aktiveret og indstillet til **EveryoneInCompany.** Hvis du vil tillade, at alle, herunder anonyme brugere, kan tilmelde sig, skal du angive mødepolitikken **til Alle** ved hjælp af kommandoen Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Bemærk!** Hvis anonym deltagelse er slået fra i mødeindstillinger, kan anonyme brugere ikke deltage i webinarer. Du kan få mere at vide og aktivere denne indstilling [under Administrer mødeindstillinger i Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Hvis du vil deaktivere møderegistrering, skal du *angive AllowMeetingRegistration* til **False**.

Hvis du vil have mere at vide om, hvem der kan tilmelde sig webinarer, skal [du se Konfigurer, hvem der kan tilmelde sig webinarer.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Hvis du vil have mere at vide om indstillinger for Microsoft-lister, skal [du se Kontrolindstillinger for Microsoft-lister](/sharepoint/control-lists).
