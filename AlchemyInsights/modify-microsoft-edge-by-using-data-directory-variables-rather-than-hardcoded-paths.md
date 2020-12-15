---
title: Ændre Microsoft Edge ved hjælp af datakatalog variabler i stedet for hardcodede stier
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677331"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Ændre Microsoft Edge ved hjælp af datakatalog variabler i stedet for hardcodede stier

Hvis du for eksempel på Windows vil gemme profildata under en brugers lokale programdata i stedet for på standardplaceringen, skal du angive **UserDataDir** -politikken til **$ {local_app_data} \Edge\Profile**. 

Hvis du vil have mere at vide, skal du se [oprette Microsoft Edge User data Directory-variabler](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).