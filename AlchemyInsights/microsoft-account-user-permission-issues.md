---
title: Fejlfindingsproblem - Brugeren blev ikke fundet i mappen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702732"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Fejlfindingsproblem - Brugeren blev ikke fundet i mappen

Hvis brugerne modtager fejlmeddelelsen "Brugeren kan ikke findes" i mappen, skal du prøve igen, hvor problemtypen er Bruger, der ikke er i mappen.

Følgende trin kan udføres for at foretage fejlfinding af problemet.

- Sørg for, at den konto, der har accepteret e-mailinvitationen, er den samme konto, som bruges til at logge på senere. Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet. 

Du kan finde flere oplysninger under [Sådan</a> administrerer du aliasser for din Microsoft-konto for at administrere Microsoft 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Find hvert eller flere websteder, hvor brugeren modtager fejlen. 

Føj "/_layouts/15/people.aspx/membershipgroupid=0" (inden for dobbelttilbud) til slutningen af webstedets URL-adresse. 

Eksempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Vælg brugeren på listen.

- Klik på **Fjern brugertilladelser** fra båndet. 
-  Tilføj invitationen tilbage, og send invitationen til brugeren igen.

