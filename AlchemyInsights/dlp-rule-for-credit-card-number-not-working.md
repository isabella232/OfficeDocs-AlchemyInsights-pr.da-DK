---
title: DLP-regel for kreditkortnummer virker ikke
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679435"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemer med kreditkort numre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med kreditkort numre**

Har du problemer med forebyggelse af datatab **(DLP)** , fungerer det ikke for indhold, der indeholder et **kreditkortnummer** , når du bruger en DLP-følsom oplysningstype i O365? Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de oplysninger, der er nødvendige for at udløse DLP-politikken, når den evalueres. For en **kreditkort politik** , der er konfigureret med et tillidsniveau på 85%, evalueres følgende og skal registreres, for at reglen kan udløses:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre, som kan være formateret eller uformateret (dddddddddddddddd), og som skal bestå Luhn-testen.

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Særdeles komplekst og robust mønster, der registrerer kort fra alle større mærker i hele verden, herunder Visa, MasterCard, Opdag kort, JCB, American Express, gavekort og diner-kort.

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn kontrolsum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-politik er 85% sikker på, at den har registreret denne type af følsomme oplysninger, hvis det inden for en afstand af 300 tegn:

  - Funktionen Func_credit_card finder indhold, der svarer til mønsteret.

  - Et af følgende er sandt:

  - Der er fundet et nøgleord fra Keyword_cc_verification.

  - Der er fundet et nøgleord fra Keyword_cc_name

  - Funktionen Func_expiration_date finder en dato i det rigtige datoformat.

  - Kontrolsummen

    Eksempelvis vil følgende eksempel udløse en politik for DLP-kreditkortnummer:

  - Visa: 4485 3647 3952 7352
  
  - Udløber: 2/2009

Hvis du vil have mere at vide om, hvad der kræves for at få et **kreditkortnummer** til at blive registreret for dit indhold, skal du se følgende afsnit i denne artikel: [hvad de følsomme oplysningstyper ser ud efter kreditkort nr](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number) .
  
Ved hjælp af en anden indbygget type af følsomme oplysninger, skal du se følgende artikel for oplysninger om, hvad der kræves til andre typer: [hvad de følsomme oplysningstyper ser ud for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  