---
title: DLP-regel for kreditkortnummer virker ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389571"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemer med kreditkortnumre

Har du problemer med **Data tab forebyggelse (DLP)** ikke arbejder for indhold, der indeholder et **Kreditkortnummer** , når du bruger typen DLP følsomme oplysninger i O365? I så fald sikre, at indholdet indeholder de nødvendige oplysninger til at udløse den DLP-politik, når det evalueres. For eksempel for en **politik for kreditkort** , der er konfigureret med et konfidensniveau på 85%, følgende evalueres, og skal registreres for reglen, der udløser:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre, hvilket kan være formateret eller uformateret (dddddddddddddddd) og skal bestå testen Luhn.

- **[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Meget komplekse og robust mønster, som registrerer kort fra alle større mærker i hele verden, herunder Visa, MasterCard, opdage Card, JCB, American Express, gavekort og diner kort.

- **[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-kontrolsum

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-politik er 85% sikker på, at det har fundet denne type af følsomme oplysninger, hvis, inden for en afstand af 300 tegn:

  - Funktionen Func_credit_card søger efter indhold, der svarer til mønsteret.

  - En af følgende er sandt:

  - Der findes et nøgleord fra Keyword_cc_verification.

  - Der findes et nøgleord fra Keyword_cc_name

  - Funktionen Func_expiration_date findes en dato i det rigtige format.

  - Kontrolsummen overføres

    For eksempel vil følgende eksempel udløse en DLP kreditkort nummer politik:

  - Visum: 4485 3647 3952 7352
  
  - Udløber: 2-2009

Yderligere oplysninger om, hvad der kræves for et **Kreditkortnummer** og registreres af dit indhold, kan du se følgende afsnit i denne artikel: [Hvad den følsomme oplysningstyper søge efter kreditkort #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Bruge en anden indbygget følsomme oplysninger, se følgende artikel for at få oplysninger om hvad der kræves for andre typer: [Hvad den følsomme oplysningstyper søge efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  