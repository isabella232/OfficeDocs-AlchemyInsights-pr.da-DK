---
title: Foretage fejlfinding af problemet - brugeren blev ikke fundet i mappe
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544857"
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

