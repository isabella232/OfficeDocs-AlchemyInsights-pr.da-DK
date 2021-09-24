---
title: Det er ikke muligt at tilføje en konto efter opgradering til macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506322"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Det er ikke muligt at tilføje en konto efter opgradering til macOS 11.6 Big Sur

Når du har opgraderet til macOS 11.6, vises din OneDrive til arbejds- eller skolekonto eller din personlige OneDrive-konto muligvis ikke på listen over konti, og du kan muligvis ikke logge på en anden konto fra appen.

Der er udviklet en rettelse til dette problem. Først skal du afgøre, om du kører den enkeltstående eller appversion Store af OneDrive:

- Vælg skyen OneDrive på menulinjen for at få > **til & Indstillinger**  >  **Om**  >  . Hvis versionsnummeret ikke omfatter **(Separat), har** du appversionen Store af produktet.

Hvis du bruger den enkeltstående version af OneDrive, skal du genstarte computeren og OneDrive automatisk opdateringer til et build, hvor dette problem er løst. Hvis du vil installere buildet manuelt, skal du downloade denne [.zip-fil,](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)udpakke filen og kopiere OneDrive-appen til mappen Programmer (ved at erstatte den eksisterende OneDrive-app).

Hvis du bruger appversionen Store du overveje at installere den enkeltstående version af OneDrive. Denne version fungerer på samme måde som App Store-versionen, men giver Microsoft mulighed for at tilbyde opdateringer hurtigere til brugerne og forbinde dem til en version, der indeholder en rettelse til dette problem.

1. Download den enkeltstående version af [OneDrive, der indeholder rettelsen](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. Udpakke filen, og kopiér OneDrive appen til mappen Programmer (ved at erstatte den eksisterende OneDrive app).

Hvis du skal bruge App Store-versionen, skal du vente på, Store frigiver en version af appen, der indeholder rettelsen. Desværre kan Microsoft ikke oplyse en anslået dato for en fast version, der skal frigives fra app-Store.


