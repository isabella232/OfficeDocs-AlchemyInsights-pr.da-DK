---
title: DLP fungerer ikke som forventet
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079696"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfiguration af DLP**

Har du problemer med **forebyggelse af datatab (DLP)** i Office 365 fungerer ikke som forventet? Hvis det er ja, skal du sørge for, at din **DLP-politik** er konfigureret korrekt, og at dine data indeholder det, **som DLP-politikken** leder efter, når den evalueres.
  
DLP-politikker giver dig mulighed for at identificere og beskytte følsomme oplysninger i din organisation. Brug oplysningerne her til at konfigurere [DLP-politikker.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Hvad DLP-politikker søger efter**
  
Når du bruger **de indbyggede følsomme oplysningstyper** i Security and Compliance Centers, leder DLP-politikker efter bestemte mønstre og elementer, når du registrerer disse følsomme typer.
  
- **Indbyggede typer af følsomme oplysninger**

    Du kan finde oplysninger om de indbyggede følsomme typer, og hvad en DLP-politik søger efter, når du registrerer typen Følsom, under: Hvad typerne af følsomme oplysninger [søger efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Brugerdefinerede typer af følsomme oplysninger**

    Hvis du forsøger at oprette brugerdefinerede typer af følsomme oplysninger, kan du bruge følgende artikel til at få oplysninger om, hvordan du opretter en brugerdefineret følsom type: Opret en brugerdefineret type [af følsomme oplysninger.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Test en DLP-politik**

Hvis du vil teste dine data med en indbygget eller brugerdefineret type af følsomme oplysninger, skal du bruge indstillingen **Testtype** under **Klassificeringer Følsomme**  >  **oplysningstyper**. Få mere at vide under [Test brugerdefinerede typer af følsomme oplysninger](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få indsigt i følsomme data med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se specifikke detaljer om begivenheden med en [hændelsesrapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
