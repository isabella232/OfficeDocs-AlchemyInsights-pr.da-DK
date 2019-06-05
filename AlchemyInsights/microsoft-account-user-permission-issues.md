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
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717341"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Foretage fejlfinding af problemet - brugeren blev ikke fundet i mappe

<p>Hvis brugere får vist fejlmeddelelsen <strong> &ldquo; &hellip;brugeren kan&rsquo;t findes i mappen. Prøv igen,&hellip; </strong> hvor problemtypen er <strong> &ldquo;brugeren ikke i directory.&rdquo;</strong>, kan fuldføres følgende trin for at foretage fejlfinding af problemet.</p> <ol> <li>Sikre, at den konto, der accepteres e-mail-invitationen er den samme konto, der bruges til at logge på senere. Kontroller, at brugeren bruger den samme konto til at acceptere invitationen og logge på webstedet. <br /><br />For flere oplysninger se <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">Sådan administreres aliaser til din Microsoft-konto</a> til at administrere Office 365-logon. <br /><br /></li> <li>Gå til hver enkelt eller flere steder, hvor brugeren modtager fejlen. <br /><br />en. Tilføj <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (inden for de dobbelte anførselstegn) i slutningen af URL-adressen til webstedet. <br /><br />Eksempel: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Vælg brugeren på listen. <br /><br />c. Klik på <strong>Fjern brugertilladelser på båndet</strong>. <br /><br />d. Tilføj brugeren igen og sende invitationen til brugeren.</li> </ol>

