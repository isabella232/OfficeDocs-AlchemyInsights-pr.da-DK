---
title: Fejlfinding af problem – Brugeren blev ikke fundet i kataloget
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098164"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Fejlfinding af problem – Brugeren blev ikke fundet i kataloget

Hvis brugerne modtager fejlmeddelelsen "Brugeren blev ikke fundet" i kataloget, skal du prøve igen, hvor Problemtype er Bruger ikke i kataloget.

Følgende trin kan udføres for at foretage fejlfinding af problemet.

- Kontrollér, at kontoen, der har accepteret invitationen via mail, er den samme konto, der bruges til at logge på senere. Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet. 

Du kan få mere at vide [under Sådan administrerer du aliasser for din </a> Microsoft-konto for at administrere Microsoft 365 logon.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Gå til hvert eller flere websteder, hvor brugeren modtager fejlen. 

Tilføj "/_layouts/15/people.aspx/membershipgroupid=0" (i dobbelte anførselstegn) til slutningen af webstedets URL-adresse. 

Eksempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Vælg brugeren på listen.

- Klik **på Fjern brugertilladelser** fra båndet. 
-  Tilføj brugeren igen, og afsend invitationen igen til brugeren.

