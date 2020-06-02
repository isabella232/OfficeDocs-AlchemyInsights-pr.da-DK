---
title: DLP-regel for kreditkortnummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507400"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemer med kreditkortnumre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med kreditkortnumre**

Har du problemer med **Forebyggelse af datatab (DLP),** der ikke arbejder for indhold, der indeholder et **kreditkortnummer,** når du bruger en DLP-følsom oplysningstype i O365? Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger for at udløse DLP-politikken, når den evalueres. For en **kreditkortpolitik,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks.
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre, der kan formateres eller ikke er formateret (dddddddddddddddddd) og skal bestå Luhn-testen.

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Meget komplekst og robust mønster, der registrerer kort fra alle større mærker verden over, herunder Visa, MasterCard, Discover Card, JCB, American Express, gavekort og dinerkort.

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn-kontrolsummen

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-politik er 85 % sikker på, at den registreres denne type følsomme oplysninger, hvis den er i nærheden af 300 tegn:

  - Funktionen finder Func_credit_card indhold, der svarer til mønsteret.

  - Et af følgende er sandt:

  - Der blev fundet et nøgleord fra Keyword_cc_verification.

  - Der blev fundet et nøgleord fra Keyword_cc_name

  - Funktionen Func_expiration_date finder en dato i det rigtige datoformat.

  - Kontrolsummet passerer

    Følgende eksempel udløser f.eks.

  - Visum: 4485 3647 3952 7352
  
  - Udløber: 2/2009

Du kan finde flere oplysninger om, hvad der kræves for at få registreret et **kreditkortnummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme informationstyper søger efter kreditkort#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Brug af en anden indbygget følsom oplysningstype i følgende artikel for at få oplysninger om, hvad der kræves til andre typer: [Hvad de følsomme oplysninger søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  