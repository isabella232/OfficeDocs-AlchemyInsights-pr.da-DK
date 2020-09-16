---
title: Teams tillader eller deaktiverer IP-video
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670178"
---
# <a name="teams-allow-or-disable-ip-video"></a>Teams tillader eller deaktiverer IP-video

**Ændre eller oprette en møde politik**

Hvis du vil ændre eller oprette en møde politik, skal du gå til **Microsoft teams Administrationscenter > møder > møde politikker**. Vælg en politik fra listen eller klik på **Tilføj**. Hvis du opretter en ny politik, skal du tilføje et navn og en beskrivelse. Navnet må ikke indeholde specialtegn eller være længere end 64 tegn. Vælg dine indstillinger, og klik derefter på **Gem**.

Antag f. eks., at du har mange brugere, og du vil begrænse den mængde båndbredde, som deres møde kræver. Du skal oprette en ny brugerdefineret politik kaldet "begrænset båndbredde" og deaktivere de følgende indstillinger:

Under **lyd og video**:

- Deaktiver Tillad optagelse i skyen.
- Deaktiver Tillad IP-video.

Tildel derefter politikken til brugerne.

**Tildel en mødepolitik til brugere**

1. I venstre navigationsrude i Microsoft Teams Administration skal du gå til **Brugere **og derefter klikke på brugeren.
2. Markér brugeren ved at klikke til venstre for brugernavnet, og klik derefter på **Rediger indstillinger**.
3. Under **møde politik**skal du vælge den politik, du vil tildele, og derefter klikke på **Anvend**.

Du kan finde flere oplysninger i [administrere møde politikker i teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
