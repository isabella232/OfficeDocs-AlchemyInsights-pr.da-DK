---
title: DLP-regel for amerikanske bankkontonummer fungerer ikke
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005012"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemer med amerikanske bankkontonumre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med amerikanske bankkontonumre**

Har du problemer med forebyggelse af datatab **(DLP)** ikke for indhold, der indeholder et amerikansk bankkontonummer, når du bruger en DLP-type af følsomme oplysninger i O365?  Hvis det er ja, skal du sikre dig, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken leder efter, når den evalueres.
  
Eksempelvis evalueres  følgende for en amerikansk politik for bankkontonummer, der er konfigureret med et tillidsniveau på 85 %, og den skal registreres, for at reglen udløser:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 fortløbende cifre.

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen Kontrolsum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-politik er 75 % sikker på, at den har registreret denne type af følsomme oplysninger, inden for en afstand af 300 tegn:

  - Regulære udtryk finder Regex_usa_bank_account_number, der svarer til mønsteret

  - Der er fundet Keyword_usa_Bank_Account nøgleord.

    Følgende eksempel udløser f.eks. politikken for amerikanske **bankkontonummer:** Kontrol af kontooplysninger 78344011

Du kan finde flere oplysninger  om, hvad der [kræves, for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) at et amerikansk bankkontonummer kan findes for dit indhold, i følgende afsnit i denne artikel: Hvad typerne af følsomme oplysninger ser efter amerikanske bankkontonummer
  
Ved hjælp af en anden indbygget type af følsomme oplysninger kan du se følgende artikel for at få oplysninger om, hvad der kræves til andre typer: Det, [som typerne](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) af følsomme oplysninger søger efter
  