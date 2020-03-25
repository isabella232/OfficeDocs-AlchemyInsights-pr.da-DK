---
title: DLP-regel for kreditkortnummer fungerer ikke
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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932437"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemer med kreditkortnumre

**Vigtigt**: Mange SharePoint Online- og OneDrive-kunder kører forretningskritiske programmer mod den tjeneste, der kører i baggrunden. Disse omfatter indholdsmigrering, Forebyggelse af datatab (DLP) og sikkerhedskopieringsløsninger. I disse hidtil usete tider tager vi skridt til at sikre, at SharePoint Online- og OneDrive-tjenester forbliver meget tilgængelige og pålidelige for dine brugere, der er afhængige af tjenesten mere end nogensinde før i scenarier for fjernarbejde.

Til støtte for dette mål har vi implementeret strammere begrænsningsgrænser for baggrundsapps (migrering, DLP og backupløsninger) i dagtimerne på hverdage. Du bør forvente, at disse apps vil opnå meget begrænset gennemløb i disse tider. I løbet af aftenen og i weekenden for regionen vil tjenesten dog være klar til at behandle en betydeligt større mængde anmodninger fra baggrundsapps.

**DLP problemer med kreditkortnumre**

Har du problemer med **Forebyggelse af datatab (DLP),** der ikke fungerer for indhold, der indeholder et **kreditkortnummer,** når du bruger en DLP-følsom informationstype i O365? Hvis det er tilfældet, skal du sørge for, at indholdet indeholder de nødvendige oplysninger for at udløse DLP-politikken, når den evalueres. For en **kreditkortpolitik,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende f.eks., for at reglen udløses:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cifre, der kan formateres eller uformateret (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

- **[Mønster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Meget komplekst og robust mønster, der registrerer kort fra alle større mærker over hele verden, herunder Visa, MasterCard, Discover Card, JCB, American Express, gavekort og spisekort.

- **[Kontrolsum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn checksum

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-politik er 85 % sikker på, at den har registreret denne type følsomme oplysninger, hvis der ligger 300 tegn i nærheden af 300 tegn:

  - Funktionen Func_credit_card finder indhold, der svarer til mønsteret.

  - Et af følgende er sandt:

  - Der findes et nøgleord fra Keyword_cc_verification.

  - Der findes et nøgleord fra Keyword_cc_name

  - Funktionen Func_expiration_date finder en dato i det rigtige datoformat.

  - Kontrolsummen passerer

    Følgende eksempel udløser f.eks.

  - Visum: 4485 3647 3952 7352
  
  - Udløber: 2/2009

Du kan finde flere oplysninger om, hvad der kræves, for at der kan registreres et **kreditkortnummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad søger de følsomme informationstyper efter kreditkort#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Brug en anden indbygget type følsomme oplysninger finder du i følgende artikel for at få oplysninger om, hvad der kræves for andre typer: [Hvad de følsomme informationstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  