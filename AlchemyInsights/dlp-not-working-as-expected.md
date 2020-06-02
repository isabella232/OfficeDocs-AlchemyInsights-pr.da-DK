---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507472"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Opsætning af DLP**

Har du problemer med **forebyggelse af datatab (DLP)** i Office 365 fungerer ikke som forventet? Hvis det er tilfældet, skal du sørge for, at **DLP-politikken** er konfigureret korrekt, og at dine data indeholder det, **som DLP-politikken** søger efter, når den evalueres.
  
DLP-politikker giver dig mulighed for at identificere og beskytte følsomme oplysninger i organisationen. Hvis du vil konfigurere DLP-politikker, skal du bruge oplysningerne [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Hvad DLP-politikker søger efter**
  
Når du bruger de **indbyggede følsomme oplysningstyper** i sikkerhedscentrene, søger DLP-politikkerne efter specifikke mønstre og elementer, når disse følsomme typer registreres.
  
- **Indbyggede følsomme informationstyper**

    Du kan finde oplysninger om de indbyggede følsomme typer, og hvad en DLP-politik søger efter, når du registrerer typen Følsom, under: [Hvad de følsomme oplysningstyper søger efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Brugerdefinerede følsomme oplysningstyper**

    Hvis du forsøger at oprette brugerdefinerede følsomme oplysningstyper, skal du bruge følgende artikel til at få oplysninger om, hvordan du opretter en brugerdefineret følsom type: [Opret en brugerdefineret følsom oplysningstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Test en DLP-politik**

Hvis du vil teste dine data med en indbygget eller brugerdefineret følsom oplysningstype, skal du bruge indstillingen **Testtype** under **Klassifikationsfølsomme**  >  **oplysningstyper**. Yderligere oplysninger finder du i [Test af brugerdefinerede følsomme oplysningstyper](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få følsom dataindsigt med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se specifikke oplysninger om hændelsen med en [hændelsesrapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
