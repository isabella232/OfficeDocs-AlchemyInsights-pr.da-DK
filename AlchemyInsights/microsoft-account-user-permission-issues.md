---
title: Fejlfinding af problem-brugeren blev ikke fundet i mappen
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754186"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Fejlfinding af problem-brugeren blev ikke fundet i mappen

Selv om brugernes er modtager fejl besked "bruger kan ikke ' være oprette" i den bibliotek. Prøv igen, hvor problemtypen er bruger ikke i mappen.

Følgende trin kan udføres for at løse problemet.

- Sørg for, at den konto, der accepterede e-mailinvitationen, er den samme konto, som bruges til at logge på senere. Sørg for, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet. 

Du kan finde flere oplysninger under [Sådan administrerer du aliasser for din</a> Microsoft-konto for at administrere Office 365-logon](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Gå til hvert sted (er), hvor brugeren modtager fejlen. 

Tilføj "/_layouts/15/People.aspx/membershipgroupid = 0" (i dobbelt anførselstegn) til slutningen af webstedets URL-adresse. 

Eksempel: https:/_Lt_ "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.

- Vælg brugeren på listen.

- Klik på **Fjern brugertilladelser** fra båndet. 
-  Tilføj brugeren tilbage, og send invitationen til brugeren igen.

