---
title: Opret en mail, opfang alle
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080740"
---
# <a name="create-an-email-catch-all"></a>Opret en mail, opfang alle

Det frarådes på det kraftigste at bruge en opfangne. Det er bedre at give afsenderen en tilbagevisning, så afsenderen ved, at meddelelsen ikke kunne leveres som adresseret, så afsenderen kan handle. Du kan også begrænse den overvågede postkasse til kun at fange tidligere gyldige mailadresser. 

Enhver opfang alle postkasser modtager en hel del spam og kan blive fyldt op med tiden, hvis de ikke overvåges nøje. (Der modtager begrænsninger). 

Hvis du beslutter dig for at fortsætte, skal du følge disse trin:

1. Opret en dynamisk distributionsgruppe, & inkluderer "Alle modtagertyper".

2. Opret en dedikeret postkasse for at få mails, f.eks. catchall@domain.com.

3. For det specifikke domæne skal du indstille DomainType til "InternalRelay". Hvis du senere fjerner alle uønskede, skal du sørge for at indstille domænet tilbage til Autoritativ.

4. Opret en transportregel for mailflow på følgende måde:

    - Hvis afsenderen er "Uden for organisationen"
    - Omdiriger meddelelsen til Catchall@domain.com
    - Undtagen hvis modtageren er medlem af allusers@domain.com (Distributionsgruppe indeholder alle medlemmer)
    - Sørg for at validere, at nye postkasser føjes til den dynamiske distributionsgruppe
