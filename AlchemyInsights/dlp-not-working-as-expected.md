---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977432"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Vigtigt**: I disse hidtil usete tider bestræber vi os på at sikre, at SharePoint Online- og OneDrive-tjenesterne fastholder sin høje tilgængelighed. Hvis du ønsker flere oplysninger, skal du besøge [Midlertidige funktionsjusteringer i SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Opsætning af DLP**

Har du problemer med **Forebyggelse af datatab (DLP)** i Office 365 fungerer ikke som forventet? Hvis det er tilfældet, skal du sørge for, at **DLP-politikken** er konfigureret korrekt, og at dine data indeholder, hvad **DLP-politikken** søger efter, når den evalueres.
  
DLP-politikker giver dig mulighed for at identificere og beskytte følsomme oplysninger i organisationen. Hvis du vil konfigurere DLP-politikker, skal du bruge oplysningerne [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Hvad DLP politikker kigge efter**
  
Når dlp-politikker bruger de **indbyggede følsomme oplysningstyper** i Office 365 Security and Compliance Center, søger de specifikke mønstre og elementer, når du registrerer disse følsomme typer.
  
- **Indbyggede følsomme oplysningstyper**

    Du kan finde oplysninger om de indbyggede følsomme typer, og hvad en DLP-politik søger efter, når du registrerer typen Følsom, under: [Hvad de følsomme oplysningstyper søger efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Brugerdefinerede følsomme oplysningstyper**

    Hvis du forsøger at oprette brugerdefinerede følsomme oplysningstyper, kan du bruge følgende artikel til at få oplysninger om, hvordan du opretter en brugerdefineret følsom type: [Opret en brugerdefineret personfølsomme oplysningertype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Test en DLP-politik**

Hvis du vil teste dine data med en indbygget eller brugerdefineret følsom oplysningstype, skal du bruge indstillingen **Testtype** under **Klassifikationer** > **Følsomme oplysningstyper**. Yderligere oplysninger finder du i [Test af brugerdefinerede følsomme oplysningstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få indsigt i følsomme data med [DLP-rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Se specifikke oplysninger om hændelsen med en [hændelsesrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
