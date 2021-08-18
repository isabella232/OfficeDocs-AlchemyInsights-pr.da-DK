---
title: Send brugerdefinerede beskeder med Intune
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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086158"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Sådan sender du brugerdefinerede beskeder til brugere af administrerede iOS- og Android-enheder

Brugerdefinerede beskeder for Intune behandles af Firmaportal-appen på en brugers enhed. Appen opretter derefter pushmeddelelsen på den pågældende enhed.

Følgende er enhedsfor forudsætninger for at understøtte modtagelse af brugerdefinerede beskeder, og for at appen kan oprette pushmeddelelsen:

- Enheden skal have Firmaportal installeret.  

- Enheden skal tillade, at Firmaportal sender pushmeddelelser. Når appen er installeret eller opdateret, bliver brugeren bedt om at tillade meddelelser.

- Google Play-tjenester skal være installeret på Android-enheder.

- Enheden skal være tilmeldt Intune.

Du kan finde flere oplysninger om, hvordan du sender en meddelelse, i [funktionsdokumentationen](https://docs.microsoft.com/intune/custom-notifications).
