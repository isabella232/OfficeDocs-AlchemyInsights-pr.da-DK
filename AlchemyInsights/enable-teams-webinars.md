---
title: Aktivere Teams webinarer
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793581"
---
# <a name="enable-teams-webinars"></a>Aktivere Teams webinarer

Webinarer er aktiveret som standard. Du kan styre, hvem der kan planlægge og tilmelde dig Teams webinarer ved hjælp Teams PowerShell-kommandoer.

- Alle brugere, der kan oprette et møde, kan også oprette et webinarmøde. Hvis du vil administrere, hvem der kan planlægge Teams webinarer, skal du *bruge AllowMeetingRegistration*. 
- *WhoCanRegister er som standard* aktiveret og indstillet til **Alle**. Hvis du vil deaktivere møderegistrering, skal du *angive AllowMeetingRegistration* til **False**.

Hvis du vil ændre disse indstillinger, skal du [installere Teams PowerShell.](/microsoftteams/teams-powershell-install) Desuden håndhæves mødepolitikker i Teams webinarer. Hvis anonym deltagelse f.eks. er slået fra i mødeindstillinger, kan anonyme brugere ikke deltage i webinarer.

Hvis du vil have mere at vide om, hvem der kan tilmelde sig webinarer, skal [du se Konfigurer, hvem der kan tilmelde sig webinarer.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Hvis du vil have mere at vide om indstillinger for Microsoft-lister, skal [du se Kontrolindstillinger for Microsoft-lister](/sharepoint/control-lists).