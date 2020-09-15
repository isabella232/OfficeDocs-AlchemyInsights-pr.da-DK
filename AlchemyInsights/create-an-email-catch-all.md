---
title: Oprette en e-mail-samling
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712980"
---
# <a name="create-an-email-catch-all"></a>Oprette en e-mail-samling

Brug af en catch all er stærkt frarådet. Det er bedre at stille tilbage til afsenderen besked om, at afsenderen ved, at deres meddelelse ikke blev leveret som løst, så de kan handle. Du kan også begrænse den overvågede postkasse til kun at fange tidligere gyldige mailadresser. 

Alle catch-alle postkasser modtager en god slags spam og kan til enhver udfyldnings besked se ud, hvis den ikke er tæt overvåget. Der er grænser for modtagelse. 

Hvis du beslutter dig for at fortsætte, skal du følge disse trin:

1. Opret en dynamisk distributionsgruppe & du medtage "alle modtagertyper".

2. Opret en dedikeret postkasse til at fange mails, f. eks catchall@domain.com.

3. For det specifikke domæne skal du angive DomainType til "InternalRelay". Hvis du senere fjerner catch all, skal du sørge for at indstille domænet tilbage til autoritativ.

4. Opret en fejlfinding mailflowhttps://Configure.Office.com/scenario.aspx?SID=12-transport regel på følgende måde:

    - Hvis afsenderen er "uden for organisationen"
    - Omdiriger meddelelsen til Catchall@domain.com
    - Undtagen, hvis modtageren er medlem af allusers@domain.com (distributionsgruppe indeholder alle medlemmer)
    - Sørg for at bekræfte, at nye postkasser føjes til den dynamiske distributionsgruppe
