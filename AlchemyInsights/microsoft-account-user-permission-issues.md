---
title: Oprette og bruge en delt postkasse
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762395"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Foretage fejlfinding af problemet - brugeren blev ikke fundet i mappe

Hvis brugere får vist fejl meddelelse "bruger blev ikke fundet" i mappen. Prøv igen hvor problemtypen brugeren ikke er i mappen.

Følgende trin kan udføres for at løse problemet.

- Sikre, at den konto, der accepteres e-mail-invitationen er den samme konto, der bruges til at logge på senere. Kontroller, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet. 

Yderligere oplysninger finder du [hvordan du administrerer aliaser til din Microsoft-konto</a> til at administrere Office 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Gå til hver enkelt eller flere steder, hvor brugeren modtager fejlen. 

Føje "/ _layouts/15/people.aspx/membershipgroupid=0" (inden for de dobbelte anførselstegn) i slutningen af URL-adressen til webstedet. 

Eksempel: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Vælg brugeren på listen.

- Klik på **Fjern brugertilladelser** på båndet. 
-  Tilføj brugeren igen og sende invitationen til brugeren.

