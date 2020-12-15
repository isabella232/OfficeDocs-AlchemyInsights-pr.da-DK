---
title: Port Google Chrome-udvidelse til Microsoft Edge (chrom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677288"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Port Google Chrome-udvidelse til Microsoft Edge (chrom)

Det er nemt at [portere Google Chrome-udvidelse til Microsoft Edge (chrom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). I de fleste tilfælde er det kun minimums ændringer, der er nødvendige for at køre disse udvidelser på Microsoft Edge.

Det udvidelses-API'er og de manifest nøgler, der understøttes af Google Chrome, er kode kompatibel med Microsoft Edge. Microsoft Edge understøtter dog ikke udvidelsen APIs Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken og Chrome. instanceID.