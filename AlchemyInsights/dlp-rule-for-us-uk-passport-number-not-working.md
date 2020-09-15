---
title: DLP-regel for amerikansk/stor Passport-telefonnummer virker ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679218"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemer med DLP-US/UK Passport-numre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med amerikanske/engelske Passport-numre**

Har du problemer med forebyggelse af datatab **(DLP)** , der ikke virker for indhold, der indeholder et **amerikansk/britisk Passport-nummer** , når du bruger en DLP-følsom oplysningstype i O365? Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken ser ud, når den evalueres.
  
For eksempel på en politik om et **amerikansk/stor-telefonnummer** konfigureret med et tillidsniveau på 75% evalueres følgende og skal registreres, for at reglen kan udløses
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Ni cifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Ni fortløbende cifre

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen kontrolsum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-politik er 75% sikker på, at den har registreret denne type af følsomme oplysninger, hvis det inden for en afstand af 300 tegn:

  - Funktionen Func_usa_uk_passport finder indhold, der svarer til mønsteret.

  - Der er fundet et nøgleord fra Keyword_passport.

    Eksempelvis vil følgende eksempel udløse for det **amerikanske/engelske nummer** politik for Passport: amerikansk Passport-nummer 123456789

Hvis du vil have mere at vide om, hvad der kræves for at få en oversigt over dit indhold, skal du se følgende afsnit i denne artikel: [hvad følsomme oplysningstyper ser efter US/stor Passport-nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Ved hjælp af en anden indbygget type af følsomme oplysninger, skal du se følgende artikel for oplysninger om, hvad der kræves til andre typer: [hvad de følsomme oplysningstyper ser ud for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  