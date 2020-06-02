---
title: DLP-reglen for det amerikanske bankkontonummer fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507328"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problemer med amerikanske bankkontonumre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med amerikanske bankkontonumre**

Har du problemer med **Forebyggelse af datatab (DLP),** der ikke arbejder for indhold, der indeholder et **amerikansk bankkontonummer,** når du bruger en DLP-følsom oplysningstype i O365? Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken søger efter, når den evalueres.
  
For en politik for **et amerikansk bankkontonummer,** der er konfigureret med et konfidensniveau på 85 %, evalueres følgende og registreres, for at reglen kan udløses:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifre

- **[Mønster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 på hinanden følgende cifre.

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, der er ingen Checksum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-politik er 75 % sikker på, at den registreres denne type følsomme oplysninger, hvis den er i nærheden af 300 tegn:

  - Det regulære udtryk Regex_usa_bank_account_number finder indhold, der svarer til mønsteret

  - Der blev fundet et nøgleord fra Keyword_usa_Bank_Account.

    Følgende eksempel udløser f.eks. **US Bank Account Number**

Du kan finde flere oplysninger om, hvad der kræves for at finde et **amerikansk bankkontonummer** for dit indhold, i følgende afsnit i denne artikel: [Hvad de følsomme oplysninger søger efter amerikanske bankkontonummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Brug af en anden indbygget følsom oplysningstype i følgende artikel for at få oplysninger om, hvad der kræves til andre typer: [Hvad de følsomme oplysninger søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  