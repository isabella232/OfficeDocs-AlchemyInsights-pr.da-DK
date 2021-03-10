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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693294"
---
# <a name="fix-transport-rules"></a>Ret transportregler

En brugerdefineret regel for mailflow påvirkede denne meddelelse. Hvis du vil gennemse den nøjagtige regel, skal du gøre følgende:

1. Under Yderligere oplysninger skal du **notere** **GUID'et** eller **politiknavnet i indsendelsesresultaterne.**
2. Start Shell til Exchange-administration. Du kan finde flere oplysninger [i Åbn Shell til Exchange-administration.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Kør denne kommando (ved hjælp af GUID fra din indsendelse):  **Get-TransportRule -identity "GUID" | fl * Beskrivelse***
4. Gennemgå beskrivelsen for at se de konfigurerede betingelser, der har påvirket meddelelsen.

Du kan få mere at vide [under Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
