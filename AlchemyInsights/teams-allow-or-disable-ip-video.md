---
title: Teams tillade eller deaktivere IP-video
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: ad60225e5deee4a37831a3145d37916c9ce849f9f4cf475dce4c9a6210f83af9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940633"
---
# <a name="teams-allow-or-disable-ip-video"></a>Teams tillade eller deaktivere IP-video

**Ændre eller oprette en mødepolitik**

Hvis du vil ændre eller oprette en mødepolitik, skal Microsoft Teams Administration **> Møder > Mødepolitikker.** Vælg en politik fra listen eller klik på **Tilføj**. Hvis du opretter en ny politik, skal du tilføje et navn og en beskrivelse. Navnet må ikke indeholde specialtegn eller være længere end 64 tegn. Vælg dine indstillinger, og klik derefter på **Gem**.

Lad os f.eks. sige, at du har mange brugere, og du vil begrænse mængden af båndbredde, som deres møde kræver. Du skal oprette en ny brugerdefineret politik kaldet "begrænset båndbredde" og deaktivere de følgende indstillinger:

Under **lyd og video**:

- Deaktiver Tillad optagelse i skyen.
- Deaktiver Tillad IP-video.

Tildel derefter politikken til brugerne.

**Tildel en mødepolitik til brugere**

1. I venstre navigationsrude i Microsoft Teams Administration skal du gå til **Brugere** og derefter klikke på brugeren.
2. Markér brugeren ved at klikke til venstre for brugernavnet, og klik derefter på **Rediger indstillinger**.
3. Under **Mødepolitik skal** du vælge den politik, du vil tildele, og derefter klikke på **Anvend**.

Du kan finde flere oplysninger [i Administrere mødepolitikker i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
