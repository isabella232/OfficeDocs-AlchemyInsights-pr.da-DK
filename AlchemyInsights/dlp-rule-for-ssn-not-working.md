---
title: DLP-regel for CPR virker ikke
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679363"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problemer med sociale sikkerheds numre

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problemer med CPR**

Har du problemer med forebyggelse af datatab **(DLP)** , fungerer det ikke for indhold, der indeholder et **CPR-nummer (CPR)** , når du bruger en følsom oplysningstype i Microsoft 365? Hvis det er tilfældet, skal du sørge for, at dit indhold indeholder de nødvendige oplysninger om, hvad DLP-politikken ser ud. 
  
For en CPR-politik, der er konfigureret med et tillidsniveau på 85%, evalueres følgende og skal registreres, for at reglen udløses:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifre, som kan være i et formateret eller ikke-formateret mønster

- **[Mønster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fire funktioner ser ud efter CPR i fire forskellige mønstre:

  - Func_ssn finder CPR med en stærk formatering før 2011, der er formateret med bindestreger eller mellemrum (DDD-DD-dddd eller DDD DD dddd)

  - Func_unformatted_ssn finder CPR 2011 med en stærk formatering, der er formateret som ni fortløbende cifre (ddddddddd)

  - Func_randomized_formatted_ssn finder post-2011 CPR, der er formateret med bindestreger eller mellemrum (DDD-DD-dddd eller DDD DD dddd)

  - Func_randomized_unformatted_ssn finder post-2011 CPR, der er uformateret som ni fortløbende cifre (ddddddddd)

- **[Kontrolsum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, der er ingen kontrolsum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-politik er 85% sikker på, at den har registreret denne type af følsomme oplysninger, hvis det inden for en afstand af 300 tegn:

  - [Funktionen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finder indhold, der svarer til mønsteret.

  - Der er fundet et nøgleord fra [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Eksempler på nøgleord omfatter:  *social sikring, social sikrings nummer, soc SEC, CPR*  . Eksempelvis vil følgende eksempel udløse for DLP CPR-politikken: **CPR: 489-36-8350**
  
Du kan finde flere oplysninger om, hvad der kræves for CPR til dit indhold, i følgende afsnit i denne artikel: [hvad de følsomme oplysningstyper ser ud efter CPR](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Ved hjælp af en anden indbygget type af følsomme oplysninger, skal du se følgende artikel for oplysninger om, hvad der kræves til andre typer: [hvad de følsomme oplysningstyper ser ud for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  