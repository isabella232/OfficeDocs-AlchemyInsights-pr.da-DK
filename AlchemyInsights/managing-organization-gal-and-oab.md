---
title: Administrer organisations globale adresseliste og offlineadressekartotek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022438"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Administrer organisations globale adresseliste (GAL) og offlineadressekartotek (OAB)

En Global adresseliste (GAL) er en liste over mailaktiverede objekter (enhver type modtager, der kan modtage mail) i organisationen. En GAL oprettes automatisk i enhver organisation. Du kan oprette yderligere globale adresselister for at adskille brugerne efter organisation eller sted, men en enkelt bruger kan kun se og bruge én global adresseliste ad gangen.

Nogle mailklienter, f. eks. Outlook til Windows, henter den globale adresseliste til offlinebrug.. Dette kaldes et offlineadressekartotek (OAB). I Exchange Online opdateres et offlineadressekartotek kun én gang hver 8. time, og derefter skal klienter hente den for at opdatere deres lokale kopi af offlineadressekartoteket. Enhver modtagerændring skal først kunne ses i den globale adresseliste for at kommer over i offlineadressekartoteket.

Her er nogle af de mest almindelige procedurer for global adresseliste og offlineadressekartoteket:

- Af en række forskellige årsager kan det være en god ide, at nogle objekter skjules fra den globale adresseliste. Se [Skjul modtagere fra adresselister](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Hvis du har brug for at give bestemte grupper af brugere brugerdefinerede visninger af virksomhedens globale adresseliste, skal du se [Politikker for adressekartotek i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Opret en global adresseliste i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), og få mere at vide om, hvordan du arbejder med tilladelser for globale adresseliste, under [Adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Bemærk, at hvis du opretter nye globale adresselister, kan det også være en god ide at oprette et nyt offlineadressekartoteket. Se [Procedurer for offlineadressekartotek](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
