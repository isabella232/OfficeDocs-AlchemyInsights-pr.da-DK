---
title: DLP-regel for kreditkortnummer fungerer ikke
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005084"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problemer med kreditkortnumre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med kreditkortnumre**

Har du problemer med forebyggelse af datatab **(DLP)** ikke for indhold, der indeholder et kreditkortnummer, når du bruger en DLP-følsom oplysningstype i O365?  Hvis det er nødvendigt, skal du sikre dig, at dit indhold indeholder de nødvendige oplysninger til at udløse DLP-politikken, når den evalueres. Eksempelvis evalueres  følgende for en kreditkortpolitik, der er konfigureret med et tillidsniveau på 85 %, og den skal registreres, for at reglen udløser:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifre, som kan formateres eller ikke-formateres (ddddddddd) og skal bestå Luhn-testen.

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Meget komplekst og robust mønster, der registrerer kort fra alle større mærker over hele verden, herunder Visa, MasterCard, Discover Card, JCB, American Express, gavekort og Diner-kort.

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn-kontrolsummen

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-politik er 85 % sikker på, at den har registreret denne type af følsomme oplysninger, inden for en afstand af 300 tegn:

  - Funktionen finder Func_credit_card, der svarer til mønsteret.

  - Et af følgende er sandt:

  - Der er fundet Keyword_cc_verification nøgleord.

  - Der er fundet Keyword_cc_name nøgleord

  - Funktionen finder Func_expiration_date en dato i det rigtige datoformat.

  - Kontrolsummet består

    Følgende eksempel udløser f.eks. en nummerpolitik for DLP-kreditkort:

  - Visa: 4485 3647 3952 7352
  
  - Udløber: 2/2009

Du kan finde flere oplysninger  om, hvad der kræves for at et kreditkortnummer kan registreres for dit indhold, i følgende afsnit i denne artikel: Hvad typerne af følsomme oplysninger søger efter [Kreditkortnr.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Ved hjælp af en anden indbygget type af følsomme oplysninger kan du se følgende artikel for at få oplysninger om, hvad der kræves til andre typer: Det, [som typerne](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) af følsomme oplysninger søger efter
  