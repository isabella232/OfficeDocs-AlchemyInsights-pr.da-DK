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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707804"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfiguration af DLP**

Har du problemer med forebyggelse **af datatab (DLP)** i Office 365, der ikke fungerer som forventet? Hvis det er ja, skal du sørge for, at **din DLP-politik** er konfigureret korrekt, og at dine data indeholder det, **som DLP-politikken** leder efter, når den evalueres.
  
DLP-politikker giver dig mulighed for at identificere og beskytte følsomme oplysninger i din organisation. Brug oplysningerne her til at konfigurere [DLP-politikker.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Det søger DLP-politikker efter**
  
Når du bruger **de indbyggede følsomme oplysningstyper** i Security and Compliance Centers, leder DLP-politikker efter bestemte mønstre og elementer, når du registrerer disse følsomme typer.
  
- **Indbyggede typer af følsomme oplysninger**

    Du kan finde oplysninger om de indbyggede følsomme typer, og hvad en DLP-politik søger efter, når den følsomme type registreres, i: Hvad typerne af følsomme [oplysninger søger efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Brugerdefinerede typer af følsomme oplysninger**

    Hvis du forsøger at oprette brugerdefinerede typer af følsomme oplysninger, kan du bruge følgende artikel til at få oplysninger om, hvordan du opretter en brugerdefineret følsom type: Opret en brugerdefineret [type af følsomme oplysninger.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Test en DLP-politik**

Hvis du vil teste dine data med en indbygget eller brugerdefineret type af følsomme oplysninger, skal du bruge indstillingen **Testtype** under **Typer** af følsomme  >  **oplysninger under Klassificeringer.** Du kan finde flere oplysninger i [Test af brugerdefinerede typer af følsomme oplysninger.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Rapporter**
  
- Få indsigt i følsomme data med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se specifikke detaljer om begivenheden med en [hændelsesrapport.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
