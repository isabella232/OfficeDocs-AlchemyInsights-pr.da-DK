---
title: Ret transportregler
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034748"
---
# <a name="fix-transport-rules"></a>Ret transportregler

Denne meddelelse blev påvirket af en brugerdefineret regel for mailflow. Hvis du vil gennemse den nøjagtige regel, skal du gøre følgende:

1. I indsendelsesresultaterne under **Yderligere oplysninger** skal du notere **GUID'et** eller **politiknavnet.**
2. Start Exchange Management Shell. Du kan få mere at [vide under Åbn Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Kør denne kommando (ved hjælp af GUID fra din indsendelse):  **Get-TransportRule -identity "GUID" | fl * Beskrivelse***
4. Gennemgå beskrivelsen for at se de konfigurerede betingelser, der har påvirket meddelelsen.

Du kan få mere at vide [under Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
