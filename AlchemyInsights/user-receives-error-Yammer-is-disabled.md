---
title: Brugeren får vist fejl AADSTS7000112 Yammer er deaktiveret
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197874"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Brugeren får vist fejl AADSTS7000112 Yammer er deaktiveret

Hvis du får vist fejlmeddelelsen "AADSTS7000112: Programmet '00000005-0000-0ff1-ce00-0000000000'(Yammer) er deaktiveret", er der et problem med tjenesteproektoren i Azure AD. En administrator har muligvis deaktiveret tjenesterektoren for at blokere adgangen til Yammer.

Deaktivering af tjenesterektoren anbefales ikke og kan forårsage yderligere problemer. Du kan finde flere oplysninger om den understøttede fremgangsmåde til at blokere brugeradgang til Yammer under [Slå Yammer-adgang fra for Microsoft 365-brugere](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Sådan løser du dette problem på Azure Portal og gendanner brugeradgang til Yammer:

1.  Åbn Siden Azure Active Directory, og vælg **Virksomhedsprogrammer** under **Administrer** i venstre navigationsrude.
3.  Skriv **Office 365 Yammer** i søgefeltet, og vælg det programnavn, der skal åbnes indstillinger.
4.  Vælg **Egenskaber** under **Administrer** i venstre navigationsrude.
5.  Skal værdien **Aktiveret for brugere skal logge på til** **Ja**, og vælg derefter **Gem**.
6.  Log på Yammer igen. Du skal muligvis rydde cookies.

Du kan også køre PowerShell-kommandoer for at angive værdien. Du kan finde flere oplysninger under [fejlen "Beklager, men vi har problemer med at logge dig på", når du klikker på Yammer-feltet i Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 