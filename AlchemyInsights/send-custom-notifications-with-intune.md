---
title: Send brugerdefinerede meddelelser med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886851"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Sådan sender du brugerdefinerede meddelelser til brugerne af administrerede iOS-og Android-enheder

Brugerdefinerede meddelelser for Intune behandles af firmaets Portal-appen på en brugers enhed. Appen opretter derefter push-meddelelsen på den pågældende enhed.

Følgende er enheds forudsætninger for at understøtte modtagelse af brugerdefinerede meddelelser, og for at appen kan oprette push-meddelelsen:

- Enheden skal have appen firma Portal installeret.  

- Enheden skal tillade, at appen firma Portal sender pushmeddelelser. Når appen er installeret eller opdateret, bliver brugeren bedt om at tillade meddelelser.

- Android-enheder skal have Google Play-tjenester installeret.

- Enheden skal være tilmeldt Intune.

Yderligere oplysninger om, hvordan du sender en meddelelse, finder du i [dokumentationen til funktionen](https://docs.microsoft.com/intune/custom-notifications).
