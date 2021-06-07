---
title: Tjenesten 1048 5.7.750 er ikke tilgængelig. Klient blokeret fra at sende fra domæner, der ikke er registrerede
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774245"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750-klient er blokeret fra at sende fra et domæne, der ikke er registreret

Fejlen opstår, når der sendes en stor mængde meddelelser fra domæner, der ikke er klargjort i din lejer (tilføjet som accepterede domæner og valideret).

For at undgå denne fejl kan du bruge en certifikatbaseret mailflowforbindelse, hvor certifikatets domæne er et klargjort domæne, eller du kan klargøre alle afsendende domæner.

Se Løs problemer med levering af mail [for fejlkoderne 5.7.700 til og med 5.7.750](https://go.microsoft.com/fwlink/?linkid=2164955)i Exchange Online for at få flere oplysninger.