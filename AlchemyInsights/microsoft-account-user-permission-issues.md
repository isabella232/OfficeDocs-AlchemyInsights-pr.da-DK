---
title: Fejlfinding af problem – brugeren blev ikke fundet i katalog
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725401"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Fejlfinding af problem – brugeren blev ikke fundet i katalog

Hvis brugerne får vist fejlmeddelelsen "brugeren blev ikke fundet" i adresselisten, skal du prøve igen, hvor problemtypen ikke er på adresselisten.

Følgende trin kan udføres for at foretage fejlfinding af problemet.

- Kontrollér, at den konto, der accepterede e-mail-invitationen, er den samme konto, der bruges til at logge på senere. Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet. 

Hvis du vil have mere at vide, skal du se [Sådan administreres aliasser for din Microsoft-konto </a> til at administrere Microsoft 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Gå til hvert websted (e), hvor brugeren modtager fejlen. 

Tilføj "/_layouts/15/People.aspx/membershipgroupid = 0" (inden for dobbelte anførselstegn) i slutningen af webstedets URL-adresse. 

Eksempel: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Vælg brugeren på listen.

- Klik på **Fjern brugertilladelser** fra båndet. 
-  Tilføj brugeren tilbage og send invitationen til brugeren igen.

