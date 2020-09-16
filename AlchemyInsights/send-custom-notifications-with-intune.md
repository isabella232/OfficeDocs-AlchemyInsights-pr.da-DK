---
title: Send brugerdefinerede meddelelser til Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720640"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Sådan sender du brugerdefinerede meddelelser til brugerne af administrerede iOS-og Android-enheder

Brugerdefinerede meddelelser for Intune behandles af appen firma Portal på en brugers enhed. Appen opretter derefter push-beskeden på den pågældende enhed.

Følgende er enheds forudsætninger, der understøtter modtagelse af brugerdefinerede meddelelser, og for appen, så du kan oprette en push-besked:

- Enheden skal have appen firma Portal installeret.  

- Enheden skal give appen firma Portal besked om at sende pushmeddelelser. Når appen installeres eller opdateres, bliver brugeren bedt om at tillade meddelelser.

- Der skal være installeret Google Play Services på Android-enheder.

- Enheden skal være tilmeldt med Intune.

Du kan finde flere oplysninger, herunder hvordan du sender en meddelelse, i [dokumentationen til funktionen](https://docs.microsoft.com/intune/custom-notifications).
